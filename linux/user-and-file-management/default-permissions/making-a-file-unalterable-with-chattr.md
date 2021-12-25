
---
 autor: tuwidc
 tipo: normal
 categoría: cómo hacerlo
 etiquetas:
   - linux
   - chattr
   - inalterable
   - Terminal
   - obscura
   - ejercicio
 revisionPregunta:
   formatos:
     - llenar el vacío
   contexto: relativo
 ---

 # Hacer un archivo inalterable con `chattr`


 ---

 ## Contenido

 Puede hacer que un archivo sea inalterable para que no pueda ser cambiado o eliminado incluso por root:

 `` bash
 sudo chattr + i / ruta / a / archivo
 ''

 Después de eso, el archivo se convierte en * intocable *.

 Para hacerlo alterable nuevamente, elimine el atributo usando la bandera `-i`:

 `` bash
 sudo chattr -i / ruta / a / archivo
 ''

 Utilice la bandera `-R` para desbloquear un directorio.

 `` bash
 sudo chattr -R -i directorio /
 ''

 El equivalente de Mac es:

 `` bash
 # para "bloquear" el archivo
 chflags uchg / ruta / a / archivo
 # para desbloquear"
 chflags nouchg / ruta / a / archivo
 ''


 ---

 ## Revisión

 Hacer `enki` * archivo * inalterable:

 `` bash
 sudo ???  ???  enki
 ''

 - `chattr`
 - `+ i`
 - `-R`
 - `-Ri`
 - `-i`
