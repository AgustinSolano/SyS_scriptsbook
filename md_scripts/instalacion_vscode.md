Instalacion de VScode
=======================

A continuación, se muestra cómo instalar Visual Studio Code (VSCode) en Mac, Ubuntu y Windows, y cómo ejecutar notebooks de Jupyter utilizando el environment "mi_env".

## Instalación de Visual Studio Code

### Mac
Para instalar VSCode en Mac, sigue los siguientes pasos:

* Descarga el archivo de instalación de VSCode para Mac desde su sitio web oficial: https://code.visualstudio.com/download
* Una vez descargado, haz doble clic en el archivo descargado.
* Arrastra y suelta el archivo de instalación de VSCode en la carpeta "Aplicaciones".
* Haz clic derecho en el archivo de VSCode y selecciona "Abrir" desde el menú contextual. Esto te permitirá abrir la aplicación aunque no esté descargada de la App Store.
* Haz clic en "Abrir" en la ventana emergente para confirmar que deseas abrir la aplicación. VSCode se abrirá y estará listo para usar.

### Ubuntu
Para instalar VSCode en Ubuntu, sigue los siguientes pasos:

* Abre una terminal y ejecuta el siguiente comando para descargar la llave GPG de Microsoft:
<pre><code>wget -q https://packages.microsoft.com/keys/microsoft.asc -O- | sudo apt-key add -
</code></pre>

* Añade el repositorio de VSCode ejecutando el siguiente comando:
<pre><code>sudo add-apt-repository "deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main"
</code></pre>

* Actualiza la lista de paquetes e instala VSCode ejecutando los siguientes comandos:
<pre><code>sudo apt-get update
sudo apt-get install code
</code></pre>

* VSCode se instalará y estará listo para usar.

### Windows
Para instalar VSCode en Windows, sigue los siguientes pasos:

* Descarga el archivo de instalación de VSCode para Windows desde su sitio web oficial: https://code.visualstudio.com/download
* Haz doble clic en el archivo descargado para iniciar el instalador.
* Selecciona "Sí" en la ventana emergente para permitir que la aplicación realice cambios en tu dispositivo.
* Sigue las instrucciones del instalador para completar la instalación.
* VSCode se instalará y estará listo para usar.


## Ejecución de Notebooks de Jupyter utilizando un environment

A continuación, te mostraré cómo ejecutar notebooks de Jupyter utilizando el environment "mi_env" que creamos en el tutorial anterior.

* Abre VSCode y selecciona "File" > "Open Folder" en la barra de menú.
* Navega hasta la carpeta donde se encuentra el notebook de Jupyter que deseas abrir y selecciónala.
* En la barra lateral izquierda de VSCode, haz clic en la pestaña "Extensions" y busca "Python".
* Haz clic en "Install" para instalar la extensión de Python.
* En la barra de menú de VSCode, selecciona "View" > "Command Palette".
* Escribe "Python: Select Interpreter" en el cuadro de búsqueda y selecciónalo en la lista desplegable.
* Selecciona "Enter interpreter path" y escribe la ruta al intérprete de Python en el environment "mi_env". Por ejemplo:
<pre><code>/home/usuario/miniconda3/envs/mi_env/bin/python
</code></pre>
NOTA: esete paso va a variar segun el sistema operativo e incluso se puede seleccionar el environment de forma grafica en VScode. Recomiendo googlear para este paso.

* Haz clic en "OK"



