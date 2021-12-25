---
 autor: catalin
 tipo: normal
 categoría: cómo hacerlo
 revisionPregunta:
   formatos:
     - llenar el vacío
   contexto: relativo
 Enlaces:
   -> -
     [WOOF] (https://www.home.unix-ag.org/simon/woof.html) {sitio web}

 ---

 # Manera fácil de compartir archivos


 ---

 ## Contenido

 La transferencia de archivos en la red sin configurar software adicional se puede lograr fácilmente usando la utilidad `woof`.

 `woof` (Web Offer One File) es un script y se ejecutará en cualquier máquina con * Python * instalado.

 Para descargarlo, consulte la sección ** Más información **.

 Para compartir un archivo:

 `` bash
 ./woof / directorio / archivo

 ''

 Esto le dará una ** URL ** que se puede escribir en un navegador y comenzará la descarga.

 También puede compartir directorios:

 `` bash
 ./woof -z / directorio /
 ''

 Esto comprimirá el directorio en un tarball ** comprimido **.

 También puedes compartir el propio "woof":

 `` bash
 ./woof -s
 ''


 ---

 ## Revisión

 Una forma rápida de compartir archivos es utilizar ???  utilidad.

 - guau
 - mv
 - ssh
 - Cuota
