# git branch

`git branch` Una rama en git es simplemente un apuntador movil apuntando a uno de los commits.

`git branch -v` Muestra el ultimo commit de cada rama.

`git branch -d` elimina "Rama" si ya ha sido fusionada con la rama actual.

`git branch -D` Elimina una rama este o no fusionada con la rama actual. Se fuerza el borrado, se pierden los cambios.

`git branch --no-merged` Nos muestra la rama que no han sido fusionada a la rama actual.

`git branch --merged` Nos muestra la rama que han sido fusionadas.

`git branch --all` Nos muestra las rama que estan ocultas.

`git branch -d -r origin/master` Elimina una rama remota.
