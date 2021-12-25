---
 autor: tuwidc
 tipo: normal
 categoría: característica
 etiquetas:
   - Archivo
   - Tipo de archivo
   - Terminal
   - linux
 notas:> -

   `file` prueba cada argumento en un intento de clasificarlo.  Hay tres conjuntos
   de pruebas, realizadas en este orden: pruebas del sistema de archivos, pruebas mágicas y lenguaje
   pruebas.

   La primera prueba que se realiza correctamente hace que se imprima el tipo de archivo.
 revisionPregunta:
   formatos:
     - llenar el vacío
   contexto: relativo
 ---

 # Identificar archivos usando el comando `file`


 ---

 ## Contenido

 Identifique rápidamente el tipo de un archivo usando el comando `file`:

 `` bash
 archivo / bin / bash
 / bin / bash: ELF ejecutable LSB de 64 bits, x86-64,
  versión 1 (SYSV), vinculada dinámicamente

 archivo zte.py
 zte.py: ejecutable de texto ASCII

 archivo messaggi.zip
 messaggi.zip: datos de archivo zip, al menos
  v1.0 para extraer
 ''


 ---

 ## Revisión

 Una salida válida del comando `archivo` es:

 `` bash
 archivo script.py
 ???
 ''

 - `script.py: texto ASCII`
 - `-rw-rw-r-- 1 grupo propietario 2048 19 de noviembre de 2014 script.py`
 - `# contenido script.py`
