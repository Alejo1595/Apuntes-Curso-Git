# git log

`git log` Comando usado para ver el historial de commits.

`git log --oneline` Comando usado para ver el historial de commits en una sola linea.

`git log --graph` Comando usado para ver el historial de commits con un grafico.

`git log -n` nos muestra los ultimos n commits del historial. n --> numero de commits.

`git log --pretty=format:"%h - %an, %ar : %s"` muestra el historial con el formato que le indiquemos.

  `%h` hash del commit.
  `%an` Autor del commit.
  `%ar` tiempo que ha pasado desde que se realizo el commit.
  `%s` mensaje del commit.

` git log after "AA-MM-DD HH-MM-SS"` mostrar el historial de commits que hay despues de una fecha y hora determinada.

` git log before "AA-MM-DD HH-MM-SS"` mostrar el historial de commits que hay antes de una fecha y hora determinada.

````
se pueden combinar las banderas after y before para obtener un rango de fechas.

git log after "AA-MM-DD HH-MM-SS" --before "AA-MM-DD HH-MM-SS"
````

`git log --all` Mostrara todas las ramas del historial de commits.
