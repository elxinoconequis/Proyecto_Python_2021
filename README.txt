Fecha de Creación: 6 de Diciembre de 2021
Proyecto Python

Version de Python 3.8.1 
Objetivo: Subir de nivel en Pyhton y Git

En este caso primero hice el repositorio en la compu, paarte cree un
repositorio en línea y finalmente hice un push. Siguiendo mas o menos estos pasos:

(Pendiente)
 Pero uno de los comandos más importantes es 'remote'

Notas:

Hay que distinguir que hay repositorios locales y remoto.

**Uno de mis objetivos de este trabajo será poder retroceder entre versiones**


-------------------------------------------------------------------

<<<<< Notas >>>>>

Git y Github no es lo mismo; G

--Conceptos básicos--

Branches:

Directory: Es el folder de interés

Terminal or Command Line: Interface para comandos de texto

CLI: Command Line Interface

Headpointers:

Stage Area: Es el area anterior a hacer un commit

Work Area:

venv: (Entorno virtual)virtual environemente, para controlar las libreris y versiones de estas en nuestros proyectos. son máquiasn virtuales
*Esto sirve para instalar porque podemos isntallar las bibliotecas/paquetes que necesitemos sin afectar otros proyectos.
	Es util porque un proyecto podemos usarlo durante mucho tiempo con un paquete. y por lo tnato permite que distintos proyectos usen
	disintas verisones de un mismo paquete

	Para crearlo se utilizo el siguiente comando:
			python -m venv my-venv

	A continuación, se ejecuto el sig. comando:

			source my-venv/Scipts/activate -- pero source es un comando de linuz así que no puedo activarlo de esta manera.
	Para windows:

	C:\Users\Joaquín Fernando\Documents\Python\Proyecto_Diciembre\my-venv\Scripts\Activate.ps1
	\Ruta de donde se creo -----------------------------------------------\
	Veamos la documentación. https://code.visualstudio.com/docs/python/environments#_create-a-virtual-environment

							 https://docs.python.org/3/library/venv.html

	Para hacerlo con ANACONDA3

		https://conda.io/projects/conda/en/latest/user-guide/getting-started.html#starting-conda


Este documento es especialemente bueno.
Creación de env fuera del defaul: https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#specifying-a-location-for-an-environment

To see if a specific package is installed in an environment, in your terminal window or an Anaconda Prompt, run:

		conda list -n myenv scipy


There are a few things to be aware of when placing conda environments outside of the default envs folder.
Conda can no longer find your environment with the --name flag. You’ll generally need to pass the --prefix flag along with the environment’s full path to find the environment.

Specifying an install path when creating your conda environments makes it so that your command prompt is now prefixed with the active environment’s absolute path rather than the environment’s name.

	


Repository: El repositorio es un carpeta donde se guarda los metadaros, este
	    lo pondrmeos en la carpeta de trabajo que nos interesa.
	    
SSH Keys: Archivo que nos permite conectar con el repositorio remoto
	 En la linea de comados podemos crearla de una de las sigueintes maneras:
	> ssh-keygen -t rsa -b 4096 -C "micorreoelectronico@ejemplo.com"
	> ssh-keygen -t rsa -b 4096 -C "jf.ortega.silva@gmail.com"

	Entonces va a pedir que le pongamos nombre a nuestra llave y si le pondremos una contraseña o no.
	- yo decidi que no tuviera contraseña la llave. Se llama TestKeyJFOS

	


 <<< Shortcuts >>>
-f : force the checkout

<<< Comandos >>>

cd: cambiar directorio
	cd .. : me manda un nivel arriba de donde estoy

dir: muestra archivos


<< Git commands >>

Clone: Brings a repositoy that is hosted somewjere like Github into a  
	folder on your local machine
add : Track you files and changes in Git
commit: save your files in Git
push: uploads Git commits a to a remote repo
pull: Download changes froma  remote repo yur local machine, the opposite of push.
log:


'q' para salir de  la linea de comandos de git tras hacer un log


Lass SSH se generaron : https://phoenixnap.com/kb/generate-ssh-key-windows-10



-------
Sobre la Terminal

tenemos tre opciones que podemos hacer en el archivo laun.json

"console": "externalTerminal" / "internalConsole" / "integratedTerminal"
			abre la temrinal de windows exterior / esta va estar más limpia / esta sera sucia
			
