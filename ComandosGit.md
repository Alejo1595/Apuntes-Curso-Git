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

6. `git log` Comando usado para ver el historial de commits.

  6.1.`git log --oneline` Comando usado para ver el historial de commits en una sola linea.

  6.2.`git log --graph` Comando usado para ver el historial de commits con un grafico.

7. `git diff` Comando usado para ver los cambios que hay entre los archivos de la zona de preparación y el directorio de trabajo.
