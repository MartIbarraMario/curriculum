---
author: kapnobatai136
type: normal
category: must-know
tags:
  - introduction
  - linux
  - variables
practiceQuestion:
  formats:
    - fill-in-the-gap
    - type-in-the-gap
  context: standalone
revisionQuestion:
  formats:
    - fill-in-the-gap
  context: standalone
---

# Variables


---

## Content

Think of a *variable* as a box. 

They are used to store information. To make them easily identifiable, you put a label on them. 

Let's try creating a variable now:

```bash
best_app="Enki"
```

> 💡 Don't add any spaces around the `=` sign or you'll get an error saying `"Command not found"`.

We've taken the `"Enki"` information, and stored it in our `best_app` box:

![variable-mental-model](https://img.enkipro.com/fa537341f3027f1cea7b76ecc3398e9d.png)

To print this variable, you'd type:

```bash
echo $best_app
# Enki
```

> 💡 You need to prefix a `$` sign to the variable name to get its value

```bash
echo best_app
# best_app
```


---

## Practice

Create a variable named `good_dog` that stores `"Artemis"`, and then print it:

```bash
???="???"
echo ???
# Artemis
```

- good_dog
- Artemis
- $good_dog
- $Artemis


---

## Revision

Which of these variable declarations will throw an error in bash?

```bash
a="foobar"

b = foobar

c=foobar
```

???

- b
- a
- c



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
