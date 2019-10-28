# PDF To PNG Ubuntu
Convertir PDF a PNG en Ubuntu de forma portable y sin instalación de paquetes adicionales.

## Pasos para convertir todas las páginas
Clonamos el repositorio a nuestro equipo:

```sh
$ sudo apt-get install git
$ git clone https://github.com/rarangels/pdftopngubuntu.git
```

Al clonar, nos situamos en la carpeta descargada y ejecutamos el siguiente comando:

```sh
$ pdftoppm input.pdf outputname -png
```

En donde:

input.pdf es la ruta al archivo pdf a convertir a imágenes
outputname es el nombre con el cual saldrán las imágnes. Las imágenes salen enumeradas asi: outputname-1.png, outputname-2.png, outputname-3.png, etc... 


## Pasos para convertir una página

```sh
$ pdftoppm input.pdf outputname -png -f {page} -singlefile
```

En donde:

input.pdf es la ruta al archivo pdf a convertir a imágenes
outputname es el nombre con el cual saldrán las imágnes. Las imágenes salen enumeradas asi: outputname-1.png, outputname-2.png, outputname-3.png, etc... 
{page} corresponde al número de la página que deseas convertir, en donde 1 será la primer página.

## Pasos para especificar la resolución de la imagen

La resolución predeterminada es 150 DPI. Pero si deseas puedes agregar 

```sh
-rx {resolution} -ry {resolution}
```
Al comando. En donde:

{resolution} Equivale a la resolución deseada para la imagen.
