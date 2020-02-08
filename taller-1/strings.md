# Métodos de String

Los `String` o cadenas de texto, son demasiado comunes en JavaScript y en la programación en general, en esta sección revisaremos algunos `métodos y propiedades` muy útiles para cuando trabajes con variables de tipo `String`, veamoslas:



## Length

Supongamos que en un formulario de registro de usuarios, queremos validar si el nombre de usuario escogido cumple ciertas caracteristicas, entre las cuales está, que tenga una longitud de al menos 5 caracteres, un usuario podría escoger cualquier nombre como el del siguiente ejemplo:

```js
    let usuario = "jz";
```
La propiedad `length` nos permite conocer el tamaño o longitud del `String` en cuestión para luego tomar decisiones como informar al usuario que no se permite ese tamaño de variable, o en caso de ser un tamaño permitido continuar con el registro.

```js
    let usuario = "jz";
    
    if (usuario.length < 5 ){ //La longitud del String será de 2 caracteres
        console.log("No se permite un nombre de usuario de menos de 5 carácteres, escoja otro")
    }else{
        console.log("Puede continuar con el registro")
    }
    
```

## indexOf

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
## lastIndexOf

De la misma manera que la función anterior `lastIndexOf` nos dice la posición de un conjunto de caracteres buscados, con la diferencia que nos devuelve la posición de la última concidencia encontrada.

```js
    let recuerdos = "Mi mamá me mima"
    recuerdos.indexOf("ma") // devolvería la posición 13
```
## search

Hay otras búsquedas en las que no es suficiente definir unos caractéres, sino la selección de un patrón de búsqueda un poco mas elaborado, a este tipo de patrones se les conoce como `Expresión Regular - RegExp` que en conjunto con la función `search` nos permite realizar búsquedas mas precisas dentro de nuestros `String`.

> Para tener mas detalles sobre Expresiones Regulares ingresa  [aquí](https://developer.mozilla.org/es/docs/Web/JavaScript/Guide/Regular_Expressions)

## slice
Es una función muy útil, cuando queremos sacar una parte de un `String`, por ejemplo dividirlo a la mitad, o extraer los primeros 4 caracteres. Solo debemos decirle a la función desde cual posición desea iniciar y opcionalmente la posición final a extraer, al solo definir la posición inicial, `slice` irá hasta el último caracter de la cadena de texto.

> Ten en cuenta que el resultado no queda directamente sobre el `String` que estés manejando sino que devolverá el resultado para que lo almacenes en otra variable, por lo que la cadena de texto original, no se verá afectada.

```js
    let nombreCompleto = "Andrea Maria Suarez Alvarez"
    let nombres= nombreCompleto.slice(0,12)
    let apellidos=nombreCompleto.slice(13)
    
```
## subString
> Reto: La función `subString` es muy similar a `slice`, queda en tus manos descubrir algunas sutiles diferencias entre ambos, una pista está en escoger valores negativos, para el índice final e inicial.


## split
En ocasiones la información recibida de diferentes fuentes de datos, pueden venir dentro de un único `String` separada por un separador, aquí algunos ejemplos:

```js
    let nombres = "Diego;Andres;Yeison;Giovanny;Manuel"
    let numeros = "1,2,3,4,5,6,7,8,9"
    let animales = "perro|$gato|$vaca|$caballo" 
    
```
Para poder tratar esa información y llevarla a un arreglo o listado de datos usamos la función `split` diciendole cual es el `separador` que trae la información para ser organizada.


```js
    let nombres = "Diego;Andres;Yeison;Giovanny;Manuel"
    let numeros = "1,2,3,4,5,6,7,8,9"
    let animales = "perro|$gato|$vaca|$caballo" 
    // Los convertimos a arreglos

    let listadoNombres = nombres.split(";")
    let listadoNumeros = numeros.split(",")
    let listadoAnimales = animales.split("|$")


    console.log(listadoNombres[2])
    console.log(listadoNumeros[8])
    console.log(listadoAnimales[3])

    
```