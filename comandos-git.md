# Descripción

Dejo a mano algunos comandos de git que pueden ser útiles para quienes no estén lo suficientemente familiarizados.

## Para chequear si hay cambios
Chequear siempre antes de trabajar sobre la copia local del repositorio. El primer comando va a pedir contraseña.

		1. git fetch
		2. git status

## Actualización del directorio local
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
Para chequear si hay ramas activas

		git branch

También se puede chequear todas las ramas con este comando: 

		git ls-remote origin

Si una rama que sabemos que otra persona creó no nos aparece como activa y sabemos el nombre de la rama porque lo vemos con el comando anterior o visitando la página del repositorio, introducir el siguiente comando: 

		git fetch origin NOMBRE-DE-RAMA:NOMBRE-DE-RAMA


### Cambio de ramas
Para ir de una rama a otra

		git checkout NOMBRE-DE-RAMA

Para forzar el cambio de rama y descartar los cambios no commiteados.

		git checkout -f NOMBRE-DE-RAMA  

### Creación de rama
Para crear una nueva rama

		git checkout -b NOMBRE-DE-RAMA

### Ensamble de ramas
Para ensamblar dos ramas, primero posicionarse en la rama A, a la cual se le quiere ensamblar la rama B. 

		git merge NOMBRE-DE-RAMA-B

### Borrado de ramas
Para borrar una rama

		git branch -d NOMBRE-DE-RAMA


