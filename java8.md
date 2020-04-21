<h1>Instalación de Oracle Java 8 en Linux</h1>
<br>
¡¡Editix free 2010 solo es compatible con java 8!!
<br>
<h2>Pasos a seguir</h2>
<p>Primero, tenemos que acceder al siguiente link para descargar Java: https://www.oracle.com/java/technologies/javase-downloads.html.
<br>Bajamos al apartado de Java SE 8u251
<br>Necesitamos descargar JDK y JRE. Los tenemos en el lado derecho. Si nos fijamos, nos redirecciona a unas páginas, en donde sólo tenemos
que seleccionar el formato del paquete que descargar. En este caso, se ha usado el formato "Linux x64 Compressed Archive".
<br>
<br>ATENCION! Puede ser necesario una cuenta de oracle, la creas y podrás descargar los archivos mencionados arriba.
<h2>Instalación de JDK 8</h2>
Entramos como superusuario a una terminal. Ejecutaremos los siguientes comandos:
<br>
<code>cd Descargas/</code>
<br>
<code>mkdir /usr/jdk</code>
<br>
<code>mv jdk-8u251-linux-x64.tar.gz /usr/jdk/</code>
<br>
<code>cd /usr/jdk/</code>
<br>
<code>tar zxvf jdk-8u251-linux-x64.tar.gz</code>
<br>
Ahora tendremos el JDK de java instalado en el directorio. Podemos borrar el paquete comprimido para ahorrar espacio.
<br><br>
Introduciremos los siguientes comandos para que el sistema reconozca java:
<br>
<code>sudo update-alternatives --install "/usr/bin/java" "java" "/usr/jdk/jdk1.8.0_251/bin/java" 1500</code>
<br>
<code>sudo update-alternatives --install "/usr/bin/javac" "javac" "/usr/jdk/jdk1.8.0_251/bin/javac" 1500</code>
<br>
<code>sudo update-alternatives --install "/usr/bin/javaws" "javaws" "/usr/jdk/jdk1.8.0_251/bin/javaws" 1500</code>

</p>
