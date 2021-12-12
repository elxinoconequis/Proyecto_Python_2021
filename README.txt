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


*-----**-----**-----**-----**-----**-----**-----**-----**-----**-----*

Este es una línea agregada en el Primer-branch


	Ahora bien para hacer el merge

	la practica común de acuerdo al video es que se hace un push
	y nota el --set-upstream  = -un

	--set-upstream : sirve para para indicar en que branch

	Push the code in your local repository to GitHub

Sobre el git push :
https://www.datacamp.com/community/tutorials/git-push-pull?utm_source=adwords_ppc&utm_medium=cpc&utm_campaignid=14989519638&utm_adgroupid=127836677279&utm_device=c&utm_keyword=&utm_matchtype=&utm_network=g&utm_adpostion=&utm_creative=332602034361&utm_targetid=aud-299261629574:dsa-429603003980&utm_loc_interest_ms=&utm_loc_physical_ms=9073981&gclid=CjwKCAiAtdGNBhAmEiwAWxGcUoMhPw3pSrRSzOgSNDcWVqTjzc2kPXea_r1UF-LR9fQ1SoYYrYnQ_xoCICoQAvD_BwE

git push -u origin master is used for pushing local content to GitHub.
In the code, the origin is your default remote repository name and '-u' flag is upstream,
 which is equivalent to '-set-upstream.' and the master is the branch,
 name.upstream is the repository that we have cloned the project.

 Ejemplo para este caso: //Texo para que entre en conflicto.
						git push -u Proyecto_Python_2021 Primer-branch

						

--- Sobre los Pull Request (PR) y el merge -----

1) Pude hacerse manualmenmte en el sitio de GitHub, donde podremos agregegar comentarios

Algoq ue notaremos es que tras hacer el PR y el merge no se verá reflejado en nuestro editor de código (ambiente)
inmediatamente, porque solo esta en GitHub

	- Vamos a la branch main/master
			git checkout main
	- Luego hacemos el pull	
			git pull // como ya tenemes el upstreamo no tenemos que agregar más argumentos.

Como ya se hizo el merge, vamos a borrar la branch
			git branch -d [nombre de la branch que borrar] ' -d : delete'

2) PAra hacerlo en la terminal podemos hacer lo siguiente:


A la hora de hacer merge, puede haber conflictos si muchas personas estan trabjando sobre el mismo código.


Agrega yr hacer commit

	git commit -am "Comentario generico" // solo funciona para archivos modificados, no para archivos recién creados


entonce serira para hacer el merge local

es activar la branch princilapl y luego 		git merge [nombre de la rama a ser mezcalda]


---- Deshacer en GIT ----

Supongamos que agregamos algo al stage y que siempre no queríamos (antes de hacer un commit)

git reset: para deshacer el último cambio // no argumentes o el nombre del alchivo en cuestión

En caso de que hayamos hecho un commit que no queríamos

	git reset HEAD // HEAD: hace referencia al último commit

o bien si me quiero ir commit más atrás podnría:

	git reset HEAD~1 // alt+126 para escribri la virquilla

El hash de un commit lo podemos ver en con git log
ejemplo: 	2508c06fc5cf44a5198bd809b51f53043f2b918e

entonces podríamos tambien usar "git reset [hash]" para desahacer los cambios en el repositorio a partir de 
ese commit. Esto solo hace que dejen de estar en el stage.

Si deseamos que fueran completamente removidos

		git reset --hard [hash]






