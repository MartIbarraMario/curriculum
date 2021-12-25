
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
