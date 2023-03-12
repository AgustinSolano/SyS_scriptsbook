Instalacion de python y librerias
=======================

A continuación se presenta un tutorial que te guiará paso a paso en cómo instalar Miniconda en diferentes sistemas operativos, cómo crear y utilizar 'environments' con Conda, y cómo instalar los paquetes Numpy y Matplotlib en un nuevo environment creado con Conda.

## Instalación de Miniconda

### MacOS

* Descarga el instalador de Miniconda para MacOS desde https://docs.conda.io/en/latest/miniconda.html
* Abre el archivo descargado y sigue las instrucciones del instalador.
* Una vez completada la instalación, abre la aplicación Terminal y verifica que la instalación se haya realizado correctamente ejecutando el comando:
<pre><code>conda --version
</code></pre>

### Ubuntu
* Descarga el instalador de Miniconda para Linux desde https://docs.conda.io/en/latest/miniconda.html
* Abre una ventana de terminal y navega hasta el directorio donde se descargó el archivo. Por ejemplo, si se descargó en la carpeta "Descargas":
<pre><code>cd ~/Descargas
</code></pre>
Ejecuta el siguiente comando para instalar Miniconda (NOTA: verificar que sea la version descargada, lo que sigue es un ejemplo):
<pre><code>bash Miniconda3-latest-Linux-x86_64.sh
</code></pre>

* Sigue las instrucciones del instalador para completar la instalación.
* Una vez completada la instalación, abre una nueva ventana de terminal y verifica que la instalación se haya realizado correctamente ejecutando el comando:
<pre><code>conda --version
</code></pre>

### Windows
* Descarga el instalador de Miniconda para Windows desde https://docs.conda.io/en/latest/miniconda.html
* Abre el archivo descargado y sigue las instrucciones del instalador.
* Una vez completada la instalación, abre el programa Anaconda Prompt y verifica que la instalación se haya realizado correctamente ejecutando el comando:
<pre><code>conda --version
</code></pre>


## Creación y utilización de 'environments' con Conda

Conda te permite crear 'environments' separados para diferentes proyectos, cada uno con su propio conjunto de paquetes y dependencias. Esto puede ser útil para asegurarte de que cada proyecto tenga acceso a las versiones específicas de paquetes y dependencias que necesita, sin interferir con otros proyectos.

### Creación de un nuevo environment
Para crear un nuevo environment, abre una ventana de terminal o el programa Anaconda Prompt y ejecuta el siguiente comando:
<pre><code>conda create --name nombre_env paquete1 paquete2 ...
</code></pre>

Reemplaza "nombre_env" con el nombre que desees dar a tu nuevo environment y "paquete1 paquete2 ..." con los nombres de los paquetes que quieras instalar en el nuevo environment.

Por ejemplo, para crear un nuevo environment llamado "mi_env" con los paquetes Numpy y Matplotlib, ejecuta el siguiente comando:
<pre><code>conda create --name mi_env numpy matplotlib
</code></pre>

### Activación y desactivación de un environment
Una vez creado un nuevo environment, debes activarlo antes de poder utilizarlo. Para activar un environment, ejecuta el siguiente comando:
<pre><code>conda activate nombre_env
</code></pre>

Reemplaza "nombre_env" con el nombre del environment que quieras activar.

Para desactivar un environment, ejecuta el siguiente comando:
<pre><code>conda deactivate
</code></pre>

### Eliminación de un environment
Para eliminar un environment, ejecuta el siguiente comando:
<pre><code>conda env remove --name nombre_env
</code></pre>

Por ejemplo, para eliminar el environment "mi_env", ejecuta el siguiente comando:
<pre><code>conda env remove --name mi_env
</code></pre>


