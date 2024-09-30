## Instalar Git
Si trabajas en un entorno GNU/Linux con gestión de paquetes, esto es tan sencillo como abrir una terminal y escribir:

$ sudo apt-get install git
Para otros entornos (Windows/Mac) encontrarás ayuda en este enlace: Instalando Git

Esta guía se centrará en el uso de git en GNU/Linux, aunque los comandos y las acciones son muy similares en otros entornos (Windows/Mac) y sólo requieren pequeñas modificaciones.

## Creando un repo (local)
En este apartado veremos el primer paso trabajando con un gestor de versiones: crear un repositorio.

**Comandos básicos: git init, git clone**

## Crear un repositorio: git init
Para nuestro primer ejemplo, crearemos un repositorio local en el que empezar a trabajar. Para ello crearemos una carpeta nueva que contendrá el repositorio, y usaremos el comando 'git init':

$ mkdir test_repo
$ cd test_repo
$ git init

Tras introducir estos comandos, habremos creado un repositorio nuevo, que estará disponible de forma local.

El repositorio está vacío, así que vamos a añadir nuestro primer archivo. Abriremos un editor de texto y crearemos un archivo que se llame 'README.md'. Dentro, escribiremos la frase 'Hola, mundo!'. Para aquellos que usen GNU/Linux, esto se puede realizar usando el siguiente comando:

$ echo "Hola, mundo!" > README.md

## Añadir archivos al repositorio: git add / git commit
Este achivo está creado, pero todavía no se ha marcado para añadir al repositorio.

El comando que nos permite marcar los archivos que se añadirán al repositorio es 'git add '.

$ git add README.md
Ahora el archivo está marcado, pero todavía no se ha añadido al repositorio. Podemos comprobarlo ejecutando el comando 'git status'.

$ git status

Una vez tengamos seleccionados todos los archivos que deseamos incluir en el repositorio, hacemos un commit con el comando 'git commit'. 
Un commit guardará en estado actual de los archivos que hemos marcado, y les asignará un mensaje que indica los cambios realizados, así como un autor y un identificador.

$ git commit -m "Commit inicial"
Usando el flag '-m' podremos especificar el mensaje que indica los cambios. Si no usamos el flag '-m', nos aparecerá una pantalla donde escribir el mensaje.

Todo los cambios que hemos hecho hasta ahora han sido únicamente en el repositorio de nuestro ordenador. 
