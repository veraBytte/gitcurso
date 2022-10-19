## Lista de comandos 
* 'git log' : Me muestra la historia de todo mi proyecto
* 'git log --stat' : Me muestra la historia de todo mi proyecto y que archivos han cambiado
* 'git diff' : Me muestra estos son los cambios de lo que usted tiene en staging vs lo que usted tiene en el disco duro
* 'git diff #NumerodelCommit #NumerodelCommit': Me permite hacer una comparacion entre commits
* 'git show' : Me muestra los cambios que se hicieron en un commit
* 'git status' : Me muestra que cosas han cambiado en mi proyecto

## Staging Area
* git reset HEAD: Este es el comando para sacar archivos del área de staging. No para borrarlos ni nada de eso, solo para que los últimos cambios de estos archivos no se envíen al último commit, a menos que cambiemos de opinión y los incluyamos de nuevo en staging con git add, por supuesto.

* git rm:  Este comando nos ayuda a eliminar archivos de Git sin eliminar su historial del sistema de versiones. Esto quiere decir que si necesitamos recuperar el archivo solo debemos “viajar en el tiempo” y recuperar el último commit antes de borrar el archivo en cuestión.

Recuerda que git rm no puede usarse así nomás. Debemos usar uno de los flags para indicarle a Git cómo eliminar los archivos que ya no necesitamos en la última versión del proyecto:

* git rm --cached: Elimina los archivos de nuestro repositorio local y del área de staging, pero los mantiene en nuestro disco duro. Básicamente le dice a Git que deje de trackear el historial de cambios de estos archivos, por lo que pasaran a un estado untracked.

* git rm --force: Elimina los archivos de Git y del disco duro. Git siempre guarda todo, por lo que podemos acceder al registro de la existencia de los archivos, de modo que podremos recuperarlos si es necesario (pero debemos usar comandos más avanzados).

## Volver en el tiempo
* git reset --soft #Commit : Vuelve a ese commit pero lo que tengamos en staging sigue en staging
* git reset --hard #Commit : TODO vuelve al estado anterior
* 'git checkout #Commit' : Me permite ir y ver como era el archivo antes pero no cambia nada a no ser que haga un commit , para devolverme a la version actual utilizo git checkout master

## Ramas 

## opciones de git log

* git log --oneline - Te muestra el id commit y el título del commit.
* git log --decorate- Te muestra donde se encuentra el head point en el log.
* git log -p- Explica el número de líneas que se cambiaron y te muestra que se cambió en el contenido.
* git log --stat - Explica el número de líneas que se cambiaron brevemente.
* git shortlog - Indica que commits ha realizado un usuario, mostrando el usuario y el titulo de sus commits.
* git log --graph --oneline --decorate y
* git log --pretty=format:"%cn hizo un commit %h el dia %cd" - Muestra mensajes personalizados de los commits.
* git log -3 - Limitamos el número de commits.
* git log --after=“2018-1-2” ,
* git log --after=“today” y
* git log --after=“2018-1-2” --before=“today” - Commits para localizar por fechas.
* git log --author=“Name Author” - Commits realizados por autor que cumplan exactamente con el nombre.
* git log --grep=“INVIE” - Busca los commits que cumplan tal cual está escrito entre las comillas.
* git log --grep=“INVIE” –i- Busca los commits que cumplan sin importar mayúsculas o minúsculas.
* git log – index.html- Busca los commits en un archivo en específico.
* git log -S “Por contenido”- Buscar los commits con el contenido dentro del archivo.
* git log > log.txt - guardar los logs en un archivo txt

### Ayudas extra
* Para salir de nano o vim en Ubuntu usamos 
1.Ctrl + o
2.Enter
3.Ctrl + x

