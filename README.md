## Curso Git Desde Cero

Cambios realizados por julian1595

En caso de aparacer el siguiente error
`! [remote rejected] prueba -> prueba (permission denied)
error: failed to push some refs to 'https://github.com/julian1595/Notas-Git.git'
`
seguir los siguientes pasos.

Escriba el comando:

````
git config --global --edit
````

Agregue estas líneas de configuración al final del archivo:
````
[credential]
  helper = "Su nombre de usuario"
  useHttpPath = true
````

Cambios realizados por julian1595 desde aporte2
