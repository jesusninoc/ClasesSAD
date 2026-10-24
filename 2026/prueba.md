# Cómo hacer que Claude (y tu modelo de Ollama) controlen Chrome desde tu Mac

**Resumen:** en este artículo montamos un script con Python y Selenium que abre una web y hace clic en enlaces. Después dejamos que **Claude** lo ejecute por nosotros mediante un servidor MCP de shell. Por último, creamos una versión para que un **modelo local de Ollama** decida qué hacer con el navegador.

## Qué vamos a conseguir

1. Un script que abre `jesusninoc.com` en Chrome y hace clic en el primer enlace.
2. Que Claude Desktop pueda crear y ejecutar ese script por ti, sin que abras la Terminal.
3. Un pequeño agente en el que un modelo local de Ollama decide qué herramienta usar para controlar Chrome.

## Requisitos

- macOS con Google Chrome instalado.
- Python 3 y `pip`.
- Node.js, para los servidores MCP.
- Claude Desktop.
- Ollama con un modelo que soporte herramientas, como `llama3.1` o `qwen2.5`.

## Paso 1: controlar Chrome con Selenium

Selenium es una librería que automatiza el navegador. Desde la versión 4.6 incluye Selenium Manager, que descarga solo el `chromedriver` adecuado.

```bash
pip3 install selenium
```

Crea el archivo `abrir_primer_enlace.py`:

```python
from selenium import webdriver
from selenium.webdriver.common.by import By
from selenium.webdriver.support.ui import WebDriverWait
import time

URL = "https://www.jesusninoc.com"

# Mantiene Chrome abierto al terminar el script
opciones = webdriver.ChromeOptions()
opciones.add_experimental_option("detach", True)

driver = webdriver.Chrome(options=opciones)
driver.maximize_window()
driver.get(URL)


def primer_enlace_visible(d):
    for enlace in d.find_elements(By.CSS_SELECTOR, "a[href]"):
        try:
            if enlace.is_displayed() and enlace.get_attribute("href"):
                return enlace
        except Exception:
            continue
    return False


primer_enlace = WebDriverWait(driver, 15).until(primer_enlace_visible)

print("Haciendo clic en:", primer_enlace.get_attribute("href"))
time.sleep(1)  # pausa breve para ver qué ocurre
primer_enlace.click()
print("Página actual:", driver.current_url)
```

Ejecútalo con:

```bash
python3 abrir_primer_enlace.py
```

**Cómo funciona:**

- `detach: True` evita que Chrome se cierre cuando termina el script.
- `WebDriverWait` espera hasta 15 segundos a que aparezca un enlace.
- Elegimos el primer enlace **visible** y no simplemente el primer `<a>`. En la primera versión usé `element_to_be_clickable` y Selenium devolvió un error al comprobar un elemento nulo. Recorrer los enlaces y quedarse con el primero que `is_displayed()` lo resolvió.

**Un detalle curioso:** en `jesusninoc.com` el primer enlace visible apunta a `https://www.jesusninoc.com/#`, un enlace interno. El clic funciona, pero la URL no cambia. Si quieres un destino real, hay que elegir otro enlace, como veremos más abajo.

## Paso 2: que Claude lo ejecute por ti con MCP

**MCP (Model Context Protocol)** es el estándar que permite a Claude usar herramientas externas. Con el servidor *filesystem* Claude puede crear archivos en una carpeta de tu Mac. Pero para **ejecutar** el script necesita otro servidor: uno de shell.

Edita el archivo de configuración de Claude Desktop:

```
~/Library/Application Support/Claude/claude_desktop_config.json
```

Y añade un servidor dentro de `mcpServers`, sin tocar los que ya tengas:

```json
{
  "mcpServers": {
    "filesystem": {
      "command": "npx",
      "args": ["-y", "@modelcontextprotocol/server-filesystem", "/Users/TU_USUARIO/Documents"]
    },
    "shell": {
      "command": "npx",
      "args": ["-y", "mcp-server-commands"]
    }
  }
}
```

Cambia `TU_USUARIO` por tu usuario de macOS. Después cierra Claude del todo con **Cmd+Q** y vuelve a abrirlo.

Con esto, Claude puede:

1. Comprobar si tienes Selenium instalado y, si no, instalarlo con `pip3 install selenium`.
2. Escribir el script en tu carpeta.
3. Ejecutarlo con `python3` y leer el resultado.
4. Corregir el código si algo falla y volver a probarlo.

> **Aviso de seguridad:** un servidor MCP de shell permite ejecutar comandos en tu Mac. Lee siempre cada confirmación antes de aceptarla y no lo uses con instrucciones que no hayas escrito tú.

### Un caso real: hacer clic en las tres "publicaciones diarias"

Le pedí a Claude que hiciera clic en las tres publicaciones diarias de la portada. Tuvo que averiguar cómo estaba construida la página. Los títulos están en un `<h4>` bajo el encabezado "PUBLICACIONES DIARIAS", así que usó un XPath:

```python
XPATH = (
    "(//*[self::h1 or self::h2 or self::h3][contains(normalize-space(.), 'PUBLICACIONES DIARIAS')]"
    "/following::h4//a)[position()<=3]"
)
```

Además descubrió que los enlaces se abren en **pestañas nuevas**, así que el script tiene que detectar la pestaña nueva con `window_handles`, cambiar a ella y volver a la principal. Este ciclo de escribir, ejecutar, ver el error y corregir es lo que más aporta tener la shell conectada.

## Paso 3: hacerlo con un modelo local de Ollama

Ollama no es un cliente MCP, pero muchos modelos soportan *tool calling*: tú describes las funciones disponibles, el modelo decide cuál llamar y con qué argumentos, y tu código la ejecuta y le devuelve el resultado. Así Ollama cumple el mismo papel que Claude en el paso anterior.

Instala las dependencias y descarga un modelo:

```bash
pip3 install ollama selenium
ollama pull llama3.1
```

Crea `ollama_navegador.py`:

```python
"""
Agente local: un modelo de Ollama controla Chrome mediante herramientas (tool calling).

Uso:
    python3 ollama_navegador.py
    python3 ollama_navegador.py "abre jesusninoc.com y haz clic en las tres publicaciones diarias"
"""
import sys
import time

import ollama
from selenium import webdriver
from selenium.common.exceptions import NoSuchWindowException, TimeoutException
from selenium.webdriver.common.by import By
from selenium.webdriver.support.ui import WebDriverWait

MODELO = "llama3.1"  # cambia aquí por tu modelo (debe soportar herramientas)

XPATH_DIARIAS = (
    "(//*[self::h1 or self::h2 or self::h3][contains(normalize-space(.), 'PUBLICACIONES DIARIAS')]"
    "/following::h4//a)[position()<=3]"
)

# ---------------------------------------------------------------------------
# Navegador (se abre la primera vez que hace falta)
# ---------------------------------------------------------------------------
_driver = None
_principal = None


def _navegador():
    global _driver, _principal
    if _driver is None:
        opciones = webdriver.ChromeOptions()
        opciones.add_experimental_option("detach", True)  # Chrome sigue abierto al terminar
        _driver = webdriver.Chrome(options=opciones)
        _driver.maximize_window()
        _principal = _driver.current_window_handle
    return _driver


# ---------------------------------------------------------------------------
# Herramientas que puede usar el modelo
# ---------------------------------------------------------------------------
def abrir_web(url: str) -> str:
    """Abre una URL en Chrome."""
    if not url.startswith("http"):
        url = "https://" + url
    d = _navegador()
    d.switch_to.window(_principal)
    d.get(url)
    return f"Página abierta: {d.current_url}"


def listar_enlaces(maximo: int = 15) -> str:
    """Lista los primeros enlaces visibles de la página actual."""
    d = _navegador()
    d.switch_to.window(_principal)
    salida = []
    for e in d.find_elements(By.CSS_SELECTOR, "a[href]"):
        try:
            if e.is_displayed() and e.get_attribute("href"):
                salida.append(f"{len(salida) + 1}. {e.text.strip()[:70]} -> {e.get_attribute('href')}")
        except Exception:
            continue
        if len(salida) >= maximo:
            break
    return "\n".join(salida) or "No hay enlaces visibles."


def _clic(enlace) -> str:
    d = _navegador()
    antes = set(d.window_handles)
    d.execute_script("arguments[0].scrollIntoView({block: 'center'});", enlace)
    time.sleep(1)
    titulo = enlace.text.strip()
    try:
        enlace.click()
    except Exception:
        d.execute_script("arguments[0].click();", enlace)  # p. ej. el aviso de cookies tapa el enlace
    try:
        WebDriverWait(d, 8).until(lambda x: len(x.window_handles) > len(antes))
        nueva = [h for h in d.window_handles if h not in antes][0]
        d.switch_to.window(nueva)
        time.sleep(3)
        return f"Clic en '{titulo}'. Pestaña nueva: {d.current_url}"
    except TimeoutException:
        time.sleep(2)
        return f"Clic en '{titulo}'. Página actual: {d.current_url}"


def clic_primer_enlace() -> str:
    """Hace clic en el primer enlace visible de la página actual."""
    d = _navegador()
    d.switch_to.window(_principal)
    for e in d.find_elements(By.CSS_SELECTOR, "a[href]"):
        try:
            if e.is_displayed() and e.get_attribute("href"):
                return _clic(e)
        except Exception:
            continue
    return "No encontré ningún enlace visible."


def clic_publicaciones_diarias() -> str:
    """En jesusninoc.com, hace clic en las tres PUBLICACIONES DIARIAS de la portada, una a una."""
    d = _navegador()
    d.switch_to.window(_principal)
    if "jesusninoc.com" not in d.current_url:
        d.get("https://www.jesusninoc.com")
    WebDriverWait(d, 15).until(lambda x: len(x.find_elements(By.XPATH, XPATH_DIARIAS)) >= 3)
    resultados = []
    for i in range(3):
        try:
            d.switch_to.window(_principal)
            enlace = d.find_elements(By.XPATH, XPATH_DIARIAS)[i]
            resultados.append(f"[{i + 1}/3] " + _clic(enlace))
        except NoSuchWindowException:
            resultados.append(f"[{i + 1}/3] La ventana se cerró.")
            break
    return "\n".join(resultados)


HERRAMIENTAS = {
    "abrir_web": abrir_web,
    "listar_enlaces": listar_enlaces,
    "clic_primer_enlace": clic_primer_enlace,
    "clic_publicaciones_diarias": clic_publicaciones_diarias,
}

DEFINICION_HERRAMIENTAS = [
    {
        "type": "function",
        "function": {
            "name": "abrir_web",
            "description": "Abre una URL en Google Chrome.",
            "parameters": {
                "type": "object",
                "properties": {"url": {"type": "string", "description": "Dirección web, p. ej. https://www.jesusninoc.com"}},
                "required": ["url"],
            },
        },
    },
    {
        "type": "function",
        "function": {
            "name": "listar_enlaces",
            "description": "Lista los enlaces visibles de la página actual.",
            "parameters": {"type": "object", "properties": {}},
        },
    },
    {
        "type": "function",
        "function": {
            "name": "clic_primer_enlace",
            "description": "Hace clic en el primer enlace visible de la página actual.",
            "parameters": {"type": "object", "properties": {}},
        },
    },
    {
        "type": "function",
        "function": {
            "name": "clic_publicaciones_diarias",
            "description": "Hace clic en las tres publicaciones diarias de la portada de jesusninoc.com.",
            "parameters": {"type": "object", "properties": {}},
        },
    },
]

# ---------------------------------------------------------------------------
# Bucle del agente
# ---------------------------------------------------------------------------
SISTEMA = (
    "Eres un asistente que controla Google Chrome usando herramientas. "
    "Usa las herramientas para cumplir lo que pide el usuario, no inventes resultados "
    "y al terminar resume en español lo que hiciste."
)


def ejecutar(peticion: str, max_pasos: int = 8) -> None:
    mensajes = [
        {"role": "system", "content": SISTEMA},
        {"role": "user", "content": peticion},
    ]
    for _ in range(max_pasos):
        r = ollama.chat(model=MODELO, messages=mensajes, tools=DEFINICION_HERRAMIENTAS)
        msg = r.message
        mensajes.append(msg)

        if not msg.tool_calls:
            print("\nModelo:", msg.content)
            return

        for llamada in msg.tool_calls:
            nombre = llamada.function.name
            args = dict(llamada.function.arguments or {})
            print(f"-> {nombre}({args})")
            funcion = HERRAMIENTAS.get(nombre)
            try:
                resultado = funcion(**args) if funcion else f"Herramienta desconocida: {nombre}"
            except Exception as e:
                resultado = f"Error: {e}"
            print("   ", resultado.replace("\n", "\n    "))
            mensajes.append({"role": "tool", "tool_name": nombre, "content": str(resultado)})

    print("\nSe alcanzó el máximo de pasos.")


if __name__ == "__main__":
    texto = " ".join(sys.argv[1:]) or "Abre jesusninoc.com y haz clic en las tres publicaciones diarias"
    ejecutar(texto)
```

Ejecútalo:

```bash
python3 ollama_navegador.py
python3 ollama_navegador.py "abre jesusninoc.com y haz clic en el primer enlace"
```

### Cómo funciona el agente

1. **Las herramientas** son funciones normales de Python (`abrir_web`, `listar_enlaces`, `clic_primer_enlace`, `clic_publicaciones_diarias`) que usan Selenium.
2. **`DEFINICION_HERRAMIENTAS`** describe cada una al modelo en formato JSON: nombre, descripción y parámetros. La descripción es importante, porque el modelo la usa para decidir cuál llamar.
3. **El bucle `ejecutar`** envía la petición al modelo. Si este responde con `tool_calls`, el script ejecuta esas funciones, añade el resultado a la conversación con el rol `tool` y vuelve a llamar al modelo. Termina cuando el modelo responde con texto o se llega a `max_pasos`.
4. **`_clic`** gestiona las pestañas nuevas y usa un clic por JavaScript si el aviso de cookies tapa el enlace.

### Qué modelo elegir

- Hace falta un modelo con **soporte de herramientas**. `llama3.1` y `qwen2.5` lo tienen. Muchos modelos especializados, como los de ciberseguridad basados en DeepSeek R1, no lo soportan.
- Los modelos pequeños, como `qwen2.5:3b`, pueden equivocarse al elegir la herramienta. Con `llama3.1` de 8B suele ir mejor, pero en un portátil sin GPU potente cada paso puede tardar.

## Problemas habituales

- **`ModuleNotFoundError: No module named 'selenium'`:** ejecuta `pip3 install selenium`.
- **Se pierde la ventana de Chrome:** los enlaces que se abren en pestañas nuevas cambian la ventana activa. Por eso el script guarda la ventana principal y vuelve a ella antes de cada clic.
- **El modelo no llama a ninguna herramienta:** prueba otro modelo o haz la orden más explícita ("usa la herramienta clic_primer_enlace").
- **Claude no ve el servidor nuevo:** revisa que el JSON sea válido y reinicia con Cmd+Q, no basta con cerrar la ventana.

## Ideas para ampliarlo

- Añadir herramientas como `leer_titulo_pagina()` o `hacer_captura()`.
- Hacer que el modelo resuma el contenido de cada publicación visitada.
- Conectar el agente a un bot de Telegram para lanzar acciones desde el móvil.
