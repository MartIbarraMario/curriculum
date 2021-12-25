---
 autor: tuwidc
 tipo: normal
 categoría: característica
 etiquetas:
   - encontrar
   - golpe
   - linux
   - expresión regular
 notas: ''
 práctica Pregunta:
   formatos:
     - llenar el vacío
     - escriba en el espacio
   contexto: relativo
 revisionPregunta:
   formatos:
     - llenar el vacío
   contexto: relativo
 ---

 # Encontrar archivo con expresiones regulares


 ---

 ## Contenido

 El comando `buscar` admite expresiones regulares.  Usarlos puede ahorrarle el paso adicional de canalizar los resultados de la búsqueda a `grep`.

 Por ejemplo:

 `` texto plano
 buscar -tipo f -regex ". * / A [^ /] + \. sh $"
 ''

 se traduce como "busque cualquier archivo que comience con A y termine con una extensión sh".


 ---

 ## Práctica

 Busque archivos que tengan un título que contenga "script" como subcadena y que termine en ".py":

 `` bash
 ???  ???  ???
     ???  '. * script. * \. py'
 ''

 - `encontrar`
 - `-tipo`
 - `f`
 - `-regex`
 - `archivo`
 - `-f`
 - `fnd`


 ---

 ## Revisión

 La búsqueda de un archivo utilizando expresiones regulares se puede realizar con ???  mando.

 - `encontrar`
 - `buscar`
 - `lf`
