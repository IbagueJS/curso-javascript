# split
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
## Ejercicio

Usando las variable 'animales' del ejemplo anterior, usa la función `split` pero usando el caracter `a` como separador, muestra en pantalla el resultado en la cada una de las posiciones generadas.