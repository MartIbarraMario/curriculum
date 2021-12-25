---
 autor: tuwidc
 tipo: normal
 categoría: cómo hacerlo
 etiquetas:
   - linux
   - ssh
   - rsync
   - respaldo
   - sincronizar
   - archivo
 revisionPregunta:
   formatos:
     - llenar el vacío
   contexto: relativo
 ---

 # Preservando permisos y estructura con `rsync`


 ---

 ## Contenido

 Para copiar de forma recursiva desde un sistema remoto a su sistema local conservando los permisos y la estructura, puede usar `rsync`.  Funciona mejor para sincronizar los mismos archivos repetidamente a lo largo del tiempo:

 `` bash
 rsync -a -v -e servidor ssh: / fuente /
                            / dest /
 ''

 donde:

 `` texto plano
 -un modo de archivo;  incluye recursividad
 -v aumentar la verbosidad
 -e especifica el shell remoto a usar
 ''

 Tenga en cuenta que aquí asumimos que estamos usando autenticación basada en clave y no contraseña.


 ---

 ## Revisión

 `rsync` funciona mejor para archivos / directorios que

 ???  .

 - necesita sincronización constante
 - debe descargarse solo una vez
 - son independientes del sistema
