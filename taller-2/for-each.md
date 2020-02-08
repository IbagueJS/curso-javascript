# forEach

Método que permite ejecutar la función que se le pasa como parámetro por cada uno de los elementos de un array. 

**Sintaxis:**
```js
    miArray.forEach(miFuncion)
```

**Parámetros:** 
Este método recibe como parámetro una función que debe requerir al menos un argumento, el cual representará el valor de cada elemento  `miFuncion(valor)`. Además, esta función puede recibir de manera opcional como segundo argumento el índice `miFuncion(valor, indice)`.

**Ejemplo:**
```js
    var dias = ["lunes", "martes", "miércoles", "jueves", "viernes", "sábado", "domingo"];

    function miFuncion(valor, indice) {
    console.log("valor: " + valor + " indice: " + indice);
    }

    dias.forEach(miFuncion);
```
_Notese que al llamar la función dentro del forEach no se especifica que datos se le pasan como argumentos a la función, esto es debido a que al ser ForEach un método perteneciente a un array JavaScript por debajo le pasa el indice y el valor correspondiente a cada elemento_

## Ejercicio

Declara un array con los nombres de las personas que integran tu familia, llama este array `familia`. posteriormente, crea una función que reciba un argumento `valor` y que se encargue de imprimir en consola el valor que recibió concatenado con los apellidos de tu familia.

_Recuerda que puedes utilizar `console.log()` para imprimir en consola_
