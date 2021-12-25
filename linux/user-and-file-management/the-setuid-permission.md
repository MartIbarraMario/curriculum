---
author: tuwidc
type: normal
category: must-know
tags:
  - linux
  - terminal
  - permissions
  - chmod
  - setuid
  - deep
  - workout
practiceQuestion:
  formats:
    - fill-in-the-gap
  context: standalone
revisionQuestion:
  formats:
    - fill-in-the-gap
    - type-in-the-gap
  context: relative
---

# The `setuid` permission

---

## Content

When set-user identification (`setuid`) permission is set on an executable file, a process that runs this file is granted access based on the owner of the file, rather than the user who is running the executable file.

This special permission allows a user to access files and directories that are normally only available to the owner. For example, the `setuid` permission on the `passwd` command makes it possible for a user to change its password, assuming the permissions of the root:

```bash
ll /usr/bin/passwd
 -rwsr-xr-x 1 root /usr/bin/passwd*
```

The `s` in the permissions shows that special permissions is set.

We can set this special permissions with:

```bash
chmod +s file
```

---

## Practice

Which of the following is an alternate description of what `setuid` does?

???

- It allows users to run an executable with the permissions of the file's owner.
- It gives root privileges over the file to all other users.
- It gives elevated privileges over the file to all other users in a specific group.

---

## Revision

Use `chmod` to set the `setuid` attribute for `file`:

```bash
??? ??? ???
```

- `chmod`
- `+s`
- `file`
- `+g`
- `setuid`





---
 autor: tuwidc
 tipo: normal
 categoría: imprescindible
 etiquetas:
   - linux
   - Terminal
   - permisos
   - chmod
   - setuid
   - profundo
   - ejercicio
 práctica Pregunta:
   formatos:
     - llenar el vacío
   contexto: independiente
 revisionPregunta:
   formatos:
     - llenar el vacío
     - escriba en el espacio
   contexto: relativo
 ---

 # El permiso `setuid`

 ---

 ## Contenido

 Cuando se establece el permiso de identificación de usuario establecido (`setuid`) en un archivo ejecutable, se concede acceso a un proceso que ejecuta este archivo en función del propietario del archivo, en lugar del usuario que ejecuta el archivo ejecutable.

 Este permiso especial permite a un usuario acceder a archivos y directorios que normalmente solo están disponibles para el propietario.  Por ejemplo, el permiso `setuid` en el comando` passwd` hace posible que un usuario cambie su contraseña, asumiendo los permisos del root:

 `` bash
 ll / usr / bin / passwd
  -rwsr-xr-x 1 raíz / usr / bin / passwd *
 ''

 La `s` en los permisos muestra que se establecen permisos especiales.

 Podemos establecer estos permisos especiales con:

 `` bash
 archivo chmod + s
 ''

 ---

 ## Práctica

 ¿Cuál de las siguientes es una descripción alternativa de lo que hace "setuid"?

 ???

 - Permite a los usuarios ejecutar un ejecutable con los permisos del propietario del archivo.
 - Otorga privilegios de root sobre el archivo a todos los demás usuarios.
 - Otorga privilegios elevados sobre el archivo a todos los demás usuarios de un grupo específico.

 ---

 ## Revisión

 Utilice `chmod` para establecer el atributo` setuid` para `archivo`:

 `` bash
 ???  ???  ???
 ''

 - `chmod`
 - `+ s`
 - `archivo`
 - `+ g`
 - `setuid`