  ---
   autor: jfarmer
   tipo: normal
   categoría: imprescindible
   etiquetas:
  
     - Introducción
     - linux
     - ambiente
     - variables
     
  
   revisionPregunta:
     formatos:
       - llenar el vacío
       - escriba en el espacio
     contexto: relativo
   ---
  
   # Variables de entorno comunes
  
  
   ---
  
   ## Contenido
  
   En Linux (y otros sistemas operativos basados en Unix), las variables de entorno comunes incluyen:
  
   - `HOME`, que contiene el directorio de inicio del usuario actual.  Ese es el directorio de nivel superior para la mayoría de los demás directorios.
  
   - `PATH`, que contiene una lista de directorios donde buscar un comando.  Cuando un usuario escribe `echo` en la terminal, Linux encuentra el programa` echo` en uno de los directorios listados en `PATH` y lo ejecuta.
  
   - `PWD`, que significa ** Directorio de trabajo actual ** y contiene la ruta al directorio en el que se encuentra actualmente. Por lo general, se denomina "directorio de trabajo".
  
   - `EDITOR`, que especifica el editor de texto predeterminado.
  
   - `LANG`, que especifica el idioma del usuario, por ejemplo, un valor de` pt_BR` significa que el usuario prefiere el portugués brasileño.
  
  
   ---
  
   ## Revisión
  
   Imprime el valor de la variable ambiental `LANG`:
  
   `` bash
   ???  ???
   ''
  
   - `echo`
   - `$ LANG`
   - `lang`
   - `$ lang`
   - `ls`
