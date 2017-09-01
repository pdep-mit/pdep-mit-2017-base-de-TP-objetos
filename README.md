# Base de TP de Objetos: Music Guide

# Enunciado

El enunciado se va a ir actualizando gradualmente para cada entrega, vamos a avisar por mail cuando estén disponibles los siguientes requerimientos:

[Link al enunciado](https://docs.google.com/document/d/1PRT5VRcY8uUtQh2ZqkEqs_Bko9aFUj9IxfSDqMV-rcw/edit?usp=sharing)

# Cómo organizar la solución

El proyecto inicial cuenta con dos carpetas:
- model: acá irían los .wlk con las definiciones de objetos y clases que correspondan para resolver los requerimientos.
- test: acá irían los .wtest con los distintos casos de prueba, y también vale incluír algún .wlk en el cual definan objetos o clases con la finalidad de simplificar el testeo del TP y reutilizar lógica que no sea propia de los requerimientos.

Cada archivo .wlk puede tener más de un objeto o clase, sin embargo tener demasiados en el mismo archivo es molesto. Por eso se recomienda agruparlos en archivos distintos siguiendo el criterio que consideren más apropiado.

Luego, cuando necesiten usar las definiciones de un .wlk en otro archivo (ya sea un objeto o una clase), alcanza con incluir el import adecuado al principio.

Por ejemplo, si tienen un archivo musicos.wlk en model y quieren usar las definiciones que se encuentren allí en otro archivo, pueden importar todas las definiciones con: `import model.musicos.*`. En el caso de que el archivo desde el cual hacen el import esté dentro de la carpeta model, pueden obviar esa parte del nombre, o sea directamente `import musicos.*`.

Respecto a los casos de prueba, los mismos están separados en distintos archivos en base a la funcionalidad a la que apuntan, nuevamente para que no sea tan largo.

Se espera que reemplacen el contenido actual de cada método de test por la lógica de testeo apropiada, recordando que todos los tests tienen que tener al menos un assert.

Para correrlos todos, pueden hacer click derecho sobre el proyecto y usar la opción Run As -> All Wollok Tests in this project (aseguren que no hayan espacios en el path del proyecto, ya que esa opción hoy en día tiene problemas con eso).
