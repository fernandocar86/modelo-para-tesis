# Descripción

Dejo a mano algunos comandos útiles de git.

## Para clonar un repositorio

Abrir la terminal desde la carpeta en la que se quiera clonar el repositorio e introducir el comando clone que se genera al seleccionar la opción clone en la esquina superior derecha de donde aparece el código en la página del repositorio. Es preciso contar con git instalado para que todo funcione. Si se trabaja desde Windows, se recomienda usar la terminal git de bash, que se abre haciendo click derecho (la opción solo se encuentra disponible si git está instalado). Hacer lo mismo para introducir todo el resto de los comandos.


## Para chequear si hay cambios
Si el trabajo es colaborativo, chequear siempre antes de trabajar sobre la copia local del repositorio. El primer comando va a pedir contraseña.

		1. git fetch
		2. git status

# Actualización del directorio local
Si se encuentra que la copia local está unos commits más atrás que la del repositorio, actualizar. Para actualizar el directorio local con los cambios introducidos en el repositorio usar el siguiente comando (va a pedir contraseña)

		git pull

## Para subir cambios

En primer lugar, para agregar los archivos usar uno de los siguientes dos comandos, según se quiera especificar el nombre del archivo o no.

		git add --all
		git add NOMBRE-DE-ARCHIVO'

Luego, introducir los siguientes dos comandos. El segundo comando va a pedir contraseña

		git commit -m 'MENSAJE SOBRE LOS CAMBIOS INTRODUCIDOS'
		git push


## Gestión de ramas
### Chequeo de ramas
Para chequear si hay ramas
		git branch

### Cambio de ramas
Para ir de una rama a otra

		git checkout NOMBRE-DE-RAMA

Para forzar el cambio de rama y descartar los cambios no commiteados.

		git checkout -f NOMBRE-DE-RAMA  

### Creación de rama
Para crear una nueva rama

		git checkout -b NOMBRE-DE-RAMA

### Ensamble de ramas
Para ensamblar dos ramas, primero posicionarse en la rama A, a la cual se le quiere ensamblar la rama B. Después escribir el siguiente comando

		git merge NOMBRE-DE-RAMA-B

### Borrado de ramas
Para borrar una rama

		git branch -d NOMBRE-DE-RAMA


