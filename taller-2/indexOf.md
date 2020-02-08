# indexOf

Esta función nos sirve para buscar un caracter o conjunto de caracteres específicos en un `String`, es útil por ejemplo para encontrar palabras dentro de un texto, o simplemente para encontrar la posición de una letra en una frase.

Podríamos buscar la palabra ´Condor´ en una frase.
```js
    let frase = "Esta frase es suficiente mente larga, pero no tanto como las alas del Condor de los Andes"
    letra.indexOf("Condor") //arrojaría la posición 70 
```
O un solo caracter

```js
    let numeros = "123456789"
    numeros.indexOf("5") //arrojaría la posición 4
```
> En JavaScript la posición de los caracteres inicia desde el índice `0` es muy importante tenerlo en cuenta.

Te preguntarás que sucede en otras situaciones, como que los caracteres buscados no estén, en este caso la función devuelve `-1` y en caso de que los caracteres buscados estén mas de una vez en el `String` la función devolverá la posición de la primer incidencia, además `indexOf` es sensible a mayúsculas y minúsculas.

```js
    let recuerdos = "Mi mamá me mima"
    recuerdos.indexOf("i") // devolvería la posición 1
    recuerdos.indexOf("uo") // devolvería -1
    recuerdos.indexOf("Ma") // devolvería -1
```

## Ejercicio

Declara la variable llamada 'Abecedario' y almacena las letras del abecedario, luego muestra en pantalla la posición que ocupan las letras 't', 'm' y 'w'

