
---
 autor: tuwidc
 tipo: normal
 categoría: imprescindible
 etiquetas:
   - linux
   - permisos
   - umask
   - Terminal
   - archivos
   - obscura
   - ejercicio
   - profundo
 práctica Pregunta:
   formatos:
     - llenar el vacío
   contexto: independiente
 revisionPregunta:
   formatos:
     - llenar el vacío
   contexto: relativo
 ---

 # Entendiendo `umask`

 ---

 ## Contenido

 Cada archivo o directorio obtiene algunos permisos predeterminados cuando se crea.  Estos valores se pueden establecer usando `umask` [1].

 Como su nombre lo indica, el valor en sí es una _mask_ que _ quita_ permisos.  El permiso predeterminado que obtiene un ** directorio ** cuando se crea es 777 (rwxrwxrwx), que luego está enmascarado por el valor `umask`.

 El permiso predeterminado para ** archivos ** nuevos es 666 (rw-rw-rw-), que queda enmascarado por el valor `umask`.

 El enmascaramiento es equivalente a desactivar los bits de permiso; si el permiso aún no existe [2], la `umask` terminará sin hacer nada.  Por ejemplo, crear un nuevo archivo mientras `umask` está configurado en _111_ no cambia los permisos:

 `` bash
 rw-rw-rw-
 # el enmascaramiento de x bit aún rinde
 rw-rw-rw-
 ''

 Sin embargo, este no es el caso para un valor de "umask" de _333_, en el que los bits _w_ y _x_ están desactivados:

 `` bash
 rw-rw-rw-
 # enmascaramiento de w y x bits
 r - r - r--
 ''

 Puede comprobar el valor actual de `umask` con:

 `` bash
 umask
 0022
 # estos serían los permisos
 # para un archivo nuevo
 tocar archivo nuevo
 ls -l archivo nuevo
 -rw-r - r-- 1 grupo de usuarios 0 archivo nuevo

 # para un nuevo directorio
 mkdir nuevo-dir
 ls -l nuevo-dir
 drwxr-xr-x 2 grupo de usuarios 4096 ./
 ''

 Para cambiar la máscara de usuario de la sesión actual a `077`, ejecute:

 `` bash
 umask 077
 # o
 umask u + rwx, g-rwx, o-rwx
 # o
 umask u = rwx, g =, o =

 # + habilita permisos especificados
 # - deshabilita los permisos especificados
 # = habilita especificado, deshabilita los demás

 umask
 0700
 ''

 Para aplicar esto a todos los usuarios del sistema, debe agregarlo en el archivo `/ etc / profile` o en su archivo específico` ~ / .bashrc`.

 ---

 ## Práctica

 ¿Qué permiso predeterminado tendría un _archivo nuevo_ si `umask` es` 314` (que se traduce como `-wx - xr -`)?

 ???

 - r - rw - w-
 - r - r - r--
 - -wx-wx-w-
 - --x - x-wx

 ---

 ## Revisión

 ¿Qué valor de `umask` hace que los nuevos archivos solo sean accesibles para el usuario que los creó?

 ???

 - 077
 - 700
 - 777
 - 000

 ---

 ## Examen

 ### ¿Cómo funciona umask?

 ¿Cuál es el valor de umask, si el permiso de un archivo recién creado es `224`?

 ???

 - Los tres son válidos
 - 442
 - 552
 - 443

 ---

 ## Notas al pie

 [1: permisos]
 La _mask_ representa un valor de 4 dígitos y es un número octal válido.  Si se pasan menos dígitos como argumento, se asumen ceros a la izquierda.

 Los 3 dígitos de la derecha representan los permisos otorgados al usuario, grupo de usuarios y otros usuarios, respectivamente.

 [2: Archivos]
 En el caso de archivos, para los que el permiso x (o ejecutar) está desactivado de forma predeterminada.
