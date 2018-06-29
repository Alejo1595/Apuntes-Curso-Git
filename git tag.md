# git tag

`git tag` Lista las etiquetas. Este comando lista todas las etiquetas en orden alfabetico, el orden en el que  aparecen no tienen mayor importancia.

`Etiqueta Ligera git tag v1.1-dev` Una etiqueta ligera no es mas que un checksum de un commit guardado en un archivo, no incluye mas información para crear una etiqueta ligera no pasamos las opciones -a, -s ni -m.

`Etiqueta Anotada git tag -a v1.0 -m "Mensaje"` Se guarda en la base de datos de Git como objetos enteros. Tiene un checksum; contienen el nombre del etiquetador, correo electronico y fecha; y tiene un mensaje asociado.

`git tag -l "patron *"`Bandera que nos permite buscar etiquetas que posean un patron similar.
