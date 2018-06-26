# Comandos Git

1. `git int:`
Comando usado para inicializar el repositorio de git.

2. `git status:`
Comando de git usado para ver el estado del repositorio.

3. `git add "Nombre del archivo":` Comando de git usado para añadir un archivo del directorio de trabajo a la zona de preparación.

    3.1. `git add .` Comando de git usado para añadir todos los archivos, sin importar si se esta siguiendo o no, de la zona de trabajo a la zona de preparación.

    3.2. `git add -A` Comando de git usado para añadir solamente los archivos que se esten siguiendo de la zona de trabajo a la zona de preparación.

    3.3 `git add --amend` comando que se usa para cambiar el mensaje y la descripcion de un commit.

4. `git reset HEAD "Nombre del archivo"` Comando de git usado para sacar un arvhivo de la zona de preparación y devolverlo al directorio de trabajo.

  4.1. `git reset HEAD .` Comando de git usado para sacar todos los arvhivo de la zona de preparación y devolverlos al directorio de trabajo.

5. `git commit ` Realiza un commit con los archivos que estan en la zona de preparacion con un mensaje automatico.

  5.1. `git commit -m` Realiza un commit con los archivos que estan en la zona de preparacion añadiendole un mensaje.

  5.2. `git commit -a -m` Realiza un comit saltando el area de preparación. git Prepara automaticamente todos los archivos rastreados antes de confirmarlos.

  5.3 `git commit --amend` Rehace la confirmación. Este comando utiliza el area de preparacion para la confirmación. al final terminaras con una sola confirmación - la segunda confirmación reemplaza el resultado de la primera.

6. `git log` Comando usado para ver el historial de commits.

  6.1.`git log --oneline` Comando usado para ver el historial de commits en una sola linea.

  6.2.`git log --graph` Comando usado para ver el historial de commits con un grafico.

  6.3 `git log -n` nos muestra los ultimos n commits del historial. n --> numero de commits.

  6.4 `git log --pretty=format:"%h - %an, %ar : %s"` muestra el historial con el formato que le indiquemos.

  `%h` hash del commit.
  `%an` Autor del commit.
  `%ar` tiempo que ha pasado desde que se realizo el commit.
  `%s` mensaje del commit.

  6.5.` git log after "AA-MM-DD HH-MM-SS"` mostrar el historial de commits que hay despues de una fecha y hora determinada.

  6.6.` git log before "AA-MM-DD HH-MM-SS"` mostrar el historial de commits que hay antes de una fecha y hora determinada.

  ````
  se pueden combinar las banderas after y before para obtener un rango de fechas.

  git log after "AA-MM-DD HH-MM-SS" --before "AA-MM-DD HH-MM-SS"
  ````

  6.7 `git log --all` Mostrara todas las ramas del historial de commits.

7. `git diff` Comando usado para ver los cambios que hay entre los archivos de la zona de preparación y el directorio de trabajo.

8. `git rm` Elimina archivos rastreados del repositorio y de nuestro directorio de trabajo de manera que no aparezca la proxima vez como archivos no rastreados.

9. `git checkout "ruta del archivo"` Recupera archivos eliminados del area de trabajo.

9.1. `git checkout "hash commit"` Nos permite hacer un salto entre commits.

10. `git mv` Renombrar Archivos.

````
git mv file_from file_to
````
Equivalente a los siguientes pasos:

 1. Renombrar el archivo manualmente.
 2. `git rm` eliminar con git
 3. `git add` para agregar el archivo con el nuevo nombre.

````
Creacion de alias
git config --global alias."alias" "Comando de git"

Los alias son usados para abreviar el llamdo de un comando.

git config --list | grep alias mostrara todos los alias creados.
````
11. `git tag` Lista las etiquetas. Este comando lista todas las etiquetas en orden alfabetico, el orden en el que  aparecen no tienen mayor importancia.

11.1 `Etiqueta Ligera git tag v1.1-dev` Una etiqueta ligera no es mas que un checksum de un commit guardado en un archivo, no incluye mas información para crear una etiqueta ligera no pasamos las opciones -a, -s ni -m.

11.2 `Etiqueta Anotada git tag -a v1.0 -m "Mensaje"` Se guarda en la base de datos de Git como objetos enteros. Tiene un checksum; contienen el nombre del etiquetador, correo electronico y fecha; y tiene un mensaje asociado.

11.3`git tag -l "patron *"`Bandera que nos permite buscar etiquetas que posean un patron similar.

12. `git branch` Una rama en git es simplemente un apuntador movil apuntando a uno de los commits.

12.1 `git branch -v` Muestra el ultimo commit de cada rama.

12.2 `git branch -d` elimina "Rama" si ya ha sido fusionada con la rama actual.

12.3 `git branch -D` Elimina una rama este o no fusionada con la rama actual. Se fuerza el borrado, se pierden los cambios.

12.4 `git branch --no-merged` Nos muestra la rama que no han sido fusionada a la rama actual.

12.5 `git branch --merged` Nos muestra la rama que han sido fusionadas.

13. `git merge "otra_rama"`Este comando permite combinar dos ramas. incorpora otra_rama en la rama actual.
