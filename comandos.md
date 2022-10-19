## Lista de comandos 
* 'git log' : Me muestra la historia de todo mi proyecto
* 'git log --stat' : Me muestra la historia de todo mi proyecto y que archivos han cambiado
* 'git diff' : Me muestra estos son los cambios de lo que usted tiene en staging vs lo que usted tiene en el disco duro
* 'git diff #NumerodelCommit #NumerodelCommit': Me permite hacer una comparacion entre commits
* 'git show' : Me muestra los cambios que se hicieron en un commit
* 'git status' : Me muestra que cosas han cambiado en mi proyecto

## Staging Area
* 'git rm NombreArchivo' : Me elimina el archivo del Staging

## Volver en el tiempo
* git reset --soft #Commit : Vuelve a ese commit pero lo que tengamos en staging sigue en staging
* git reset --hard #Commit : TODO vuelve al estado anterior
* 'git checkout #Commit' : Me permite ir y ver como era el archivo antes pero no cambia nada a no ser que haga un commit , para devolverme a la version actual utilizo git checkout main

### Ayudas extra
* Para salir de nano o vim en Ubuntu usamos 
1.Ctrl + o
2.Enter
3.Ctrl + x

