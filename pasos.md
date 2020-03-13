<!DOCTYPE html>
<html>
<head>
</head>
<body>
<h1>Pasos para instalar Java 11 en Linux</h1>
<h2>1. Crear cuenta de Oracle</h2>
<p>Nos redigirimos al siguiente <a href="https://profile.oracle.com/myprofile/account/create-account.jspx">enlace </a>, nos creamos la cuenta e iniciamos sesión.</p>
<h2>2. Descargar Oracle</h2>
<p>Vamos a la siguiente página <a href="https://www.oracle.com/technetwork/java/javase/downloads/index.html"></a>y descargamos Oracle JDK 11 en formato .tar.gz. Ha de ser una versión similar a la que encontraremos en <a href="https://launchpad.net/~linuxuprising/+archive/ubuntu/java/+packages">oracle-java11-installer-local package</a>.</p>
<h2>3. Crear directorio</h2>
<p>Creamos con privilegios de superusuario la siguiente carpeta: <code>/var/cache/oracle-jdk11-installer-local/</code>y copiaremos el fichero anterior en esta carpeta.</p>
<p>Comando de ayuda:</p>
<code>sudo cp jdk-11.0.6_linux-x64_bin.tar.gz /var/cache/oracle-jdk11-installer-local/</code>
<h2>4. Añadir repositorio e instalación</h2>
<p>Para poder instalar este fichero vamos a tirar de un repositorio que almacena el instalador. Los comandos son los siguientes:</p>
<code>sudo add-apt-repository ppa:linuxuprising/java</code><br>
<code>sudo apt-get update</code><br>
<code>sudo apt install oracle-java11-installer-local</code>
<h2>5. Opcional</h2>
<p>Si queremos hacer a Oracle JDK 11 por defecto, usaremos el siguiente comando:</p>
<code>sudo apt-install oracle-java11-set-default-local</code>
</body>
</html>
