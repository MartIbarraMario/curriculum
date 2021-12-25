
---
 autor: kapnobatai136
 tipo: normal
 categoría: imprescindible
 etiquetas:
   - Introducción
   - linux
   - variables
 práctica Pregunta:
   formatos:
     - llenar el vacío
     - escriba en el espacio
   contexto: independiente
 revisionPregunta:
   formatos:
     - llenar el vacío
   contexto: independiente
 ---

 # Variables


 ---

 ## Contenido

 Piense en una * variable * como una caja.

 Se utilizan para almacenar información.  Para que sean fácilmente identificables, póngales una etiqueta.

 Intentemos crear una variable ahora:

 `` bash
 best_app = "Enki"
 ''

 > 💡 No agregue espacios alrededor del signo `=` o obtendrá un error que diga `" Comando no encontrado "`.

 Hemos tomado la información de `" Enki "` y la hemos almacenado en nuestro cuadro `best_app`:

 ! [modelo-mental-variable] (https://img.enkipro.com/fa537341f3027f1cea7b76ecc3398e9d.png)

 Para imprimir esta variable, debe escribir:

 `` bash
 echo $ best_app
 # Enki
 ''

 > 💡 Debe anteponer un signo `$` al nombre de la variable para obtener su valor

 `` bash
 echo best_app
 # best_app
 ''


 ---

 ## Práctica

 Cree una variable llamada `good_dog` que almacene` "Artemis" `, y luego imprímala:

 `` bash
 ??? = "???"
 eco ???
 # Artemisa
 ''

 - buen perro
 - Artemisa
 - $ buen_perro
 - $ Artemisa


 ---

 ## Revisión

 ¿Cuál de estas declaraciones de variables arrojará un error en bash?

 `` bash
 a = "foobar"

 b = foobar

 c = foobar
 ''

 ???

 - B
 - a
 - C
