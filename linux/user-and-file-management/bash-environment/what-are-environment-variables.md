---
author: jfarmer
type: normal
category: must-know
tags:
  - introduction
  - linux
  - environment
  - variables
practiceQuestion:
  formats:
    - fill-in-the-gap
    - type-in-the-gap
  context: standalone
revisionQuestion:
  formats:
    - fill-in-the-gap
    - type-in-the-gap
  context: standalone
---

# Environment Variables


---

## Content

An *environment variable* is a variable that is available to all the processes running in the shell.

> 💡 You can think of environment variables like global variables.

Linux contains many default environment variables.

> 💡 Environment variables are usually named with all uppercase letters to differentiate them from regular variables.

As an example, the `HOME` environment variable holds the current user's home directory.

> 💡 A "directory" is just another name for a folder.

Use the `env` command to see a list of all current environment variables:

```bash
env
# USER=enki
# HOME=/home/enki
# ... (potentially many lines)
```

If you know the name of the variable you're looking for, use the `echo` command to display it:

```shell
echo $HOME
# /home/enki
```


---

## Practice

Display a list of all the current environment variables:

```bash
???
# USER=enki
# HOME=/home/enki
# ...
```

- env
- $env
- environment
- $environment


---

## Revision

Print the value of the environmental variable `HOME` : 

```bash
??? ???
```

- `echo`
- `$HOME`
- `home`
- `$home`
- `ls`



---
 autor: jfarmer
 tipo: normal
 categoría: imprescindible
 etiquetas:
   - Introducción
   - linux
   - ambiente
   - variables
 práctica Pregunta:
   formatos:
     - llenar el vacío
     - escriba en el espacio
   contexto: independiente
 revisionPregunta:
   formatos:
     - llenar el vacío
     - escriba en el espacio
   contexto: independiente
 ---

 # Variables de entorno


 ---

 ## Contenido

 Una * variable de entorno * es una variable que está disponible para todos los procesos que se ejecutan en el shell.

 > 💡 Puede pensar en variables de entorno como variables globales.

 Linux contiene muchas variables de entorno predeterminadas.

 > 💡 Las variables de entorno generalmente se nombran con letras mayúsculas para diferenciarlas de las variables regulares.

 Como ejemplo, la variable de entorno `HOME` contiene el directorio de inicio del usuario actual.

 > 💡 Un "directorio" es simplemente otro nombre para una carpeta.

 Utilice el comando `env` para ver una lista de todas las variables de entorno actuales:

 `` bash
 env
 # USUARIO = enki
 # INICIO = / inicio / enki
 # ... (potencialmente muchas líneas)
 ''

 Si conoce el nombre de la variable que está buscando, use el comando `echo` para mostrarla:

 `` caparazón
 echo $ HOME
 # / inicio / enki
 ''


 ---

 ## Práctica

 Muestra una lista de todas las variables de entorno actuales:

 `` bash
 ???
 # USUARIO = enki
 # INICIO = / inicio / enki
 # ...
 ''

 - env
 - $ env
 - ambiente
 - $ entorno


 ---

 ## Revisión

 Imprime el valor de la variable ambiental `HOME`:

 `` bash
 ???  ???
 ''

 - `echo`
 - `$ INICIO`
 - `hogar`
 - `$ casa`
 - `ls`
