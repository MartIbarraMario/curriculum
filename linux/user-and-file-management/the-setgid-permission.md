---
author: catalin
type: normal
category: must-know
tags:
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

# The `setgid` permission

---

## Content

The `setgid` permission stands for **set group id**. This permission is similar to `setuid`, except that the process's effective group ID is changed to the _group owner_ of the file, and access of a _user_ is granted based on permissions assigned to that group. Therefore, the file belongs to the group that owns the directory, not to the user's group ownership.

When `setgid` permission is applied to a directory, files that were created in this directory belong to the group to which the directory belongs, not the group to which the creating process belongs.

To set the `setgid` bit on a file:

```bash
chmod g+s enkiscript

```

Remove the `setgid` bit:

```bash
chmod g-s enkiscript
```

To remove both `setuid` and `setgid` with octal alternative:

```bash
chmod 0777 enkiscript
```

Find all files with `setgid`:

```bash
find / -type f -perm /2000 -exec stat
    -c "%A %a %n" {} \;
```

---

## Practice

Say `team` directory belongs to group `enki` and has `setgid` permission enabled.

If a user of group `test` creates a new file in that directory, which group will own the file?

???

- enki
- test
- both groups

---

## Revision

How do you apply `setgid` bit to a file?

```bash
??? ??? myfile
```

- `chmod`
- `g+s`
- `g-s`
- `u+s`
- `a-s`
- `perm`



---
 autor: catalin
 tipo: normal
 categoría: imprescindible
 etiquetas:
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

 # El permiso `setgid`

 ---

 ## Contenido

 El permiso `setgid` significa ** set group id **.  Este permiso es similar a `setuid`, excepto que el ID de grupo efectivo del proceso se cambia al _propietario del grupo_ del archivo, y el acceso de un _usuario_ se otorga según los permisos asignados a ese grupo.  Por lo tanto, el archivo pertenece al grupo propietario del directorio, no a la propiedad del grupo del usuario.

 Cuando se aplica el permiso `setgid` a un directorio, los archivos que se crearon en este directorio pertenecen al grupo al que pertenece el directorio, no al grupo al que pertenece el proceso de creación.

 Para establecer el bit `setgid` en un archivo:

 `` bash
 chmod g + s enkiscript

 ''

 Elimina el bit `setgid`:

 `` bash
 chmod g-s enkiscript
 ''

 Para eliminar tanto `setuid` como` setgid` con la alternativa octal:

 `` bash
 chmod 0777 enkiscript
 ''

 Encuentra todos los archivos con `setgid`:

 `` bash
 buscar / -tipo f -perm / 2000 -exec stat
     -c "% A% a% n" {} \;
 ''

 ---

 ## Práctica

 Diga que el directorio `team` pertenece al grupo` enki` y tiene el permiso `setgid` habilitado.

 Si un usuario del grupo `test` crea un nuevo archivo en ese directorio, ¿qué grupo será el propietario del archivo?

 ???

 - enki
 - prueba
 - ambos grupos

 ---

 ## Revisión

 ¿Cómo se aplica el bit `setgid` a un archivo?

 `` bash
 ???  ???  mi archivo
 ''

 - `chmod`
 - `g + s`
 - `g-s`
 - `u + s`
 - `a-s`
 - `permanente`