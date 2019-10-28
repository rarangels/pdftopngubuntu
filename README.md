# PDF To PNG Ubuntu
Convertir PDF a PNG en Ubuntu

Clonamos el repositorio a nuestro equipo:

```sh
$ git clone https://github.com/rarangels/pdftopngubuntu.git
```
Al clonar, nos situamos en la carpeta descargada y ejecutamos el siguiente comando:

```sh
$ pdftoppm input.pdf outputname -png
```
En donde:

input.pdf es la ruta al archivo pdf a convertir a imágenes
outputname es el nombre con el cual saldrán las imágnes. Las imágenes salen enumeradas asi: outputname-1.png, outputname-2.png, outputname-3.png, etc... 

Es portable y no requiere instalación de paquetes adicionales.
