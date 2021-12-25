---
author: tuwidc
type: normal
category: feature
tags:
  - linux
  - terminal
  - permissions
  - sticky bit
  - deep
  - workout
revisionQuestion:
  formats:
    - fill-in-the-gap
  context: relative
---

# The `sticky bit` permission

---

## Content

The sticky bit is a permission bit that protects the files within a directory. If the directory has the sticky bit set, a file can be deleted only by the owner of the file, the owner of the directory, or by root.

This special permission prevents a user from deleting other users' files from public directories such as `/tmp`:

```bash
ll .
drwxrwxrwt 17 root root 4096 Jul 20 01:09 ./
```

The `t` in the end of the permission set means that the sticky bit is active in this folder.

To set the sticky do:

```bash
chmod +t file
```

To unset it:

```bash
chmod -t file
```

---

## Revision

The sticky bit prevents ???.

- other users from deleting the file
- the owner of the file from deleting the file
- the root from deleting the file
- the owner from moving the file


---
 autor: tuwidc
 tipo: normal
 categoría: característica
 etiquetas:
   - linux
   - Terminal
   - permisos
   - pedacito pegajoso
   - profundo
   - ejercicio
 revisionPregunta:
   formatos:
     - llenar el vacío
   contexto: relativo
 ---

 # El permiso `sticky bit`

 ---

 ## Contenido

 El bit adhesivo es un bit de permiso que protege los archivos dentro de un directorio.  Si el directorio tiene el bit adhesivo establecido, solo el propietario del archivo, el propietario del directorio o la raíz pueden eliminar un archivo.

 Este permiso especial evita que un usuario elimine los archivos de otros usuarios de directorios públicos como `/ tmp`:

 `` bash
 ll.
 drwxrwxrwt 17 raíz raíz 4096 20 de julio 01:09 ./
 ''

 La `t` al final del conjunto de permisos significa que el bit adhesivo está activo en esta carpeta.

 Para configurar el pegajoso:

 `` bash
 archivo chmod + t
 ''

 Para desarmarlo:

 `` bash
 chmod -t archivo
 ''

 ---

 ## Revisión

 La punta pegajosa previene ???.

 - otros usuarios para que no eliminen el archivo
 - el propietario del archivo para que no lo elimine
 - la raíz de eliminar el archivo
 - el propietario de mover el archivo