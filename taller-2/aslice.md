# slice

El método _slice_ retorna un nuevo arreglo seleccionando elementos de otro arreglo. Los elementos se seleccionan dada una posición _inicial_ y una _final_ del arreglo, sin embargo el valor de la posición _final_ indicada no es seleccionado.

```js
var frutas = ["Banano", "Naranja", "Limón", "Manzana", "Mango"];
var citricos = frutas.slice(1, 3);
```

_Nota: El arreglo original no es modificado_

La sintaxis del método _slice_ es la siguiente:

`array.slice(start, end)`

## Ejercicio

Genere un arreglo de cadenas de caracteres con una longitud de 10 posiciones. Utilice el método _slice_ para seleccionar los valores de las posiciones 3 a la 6 e imprima el resultado mediante `console.log()`
