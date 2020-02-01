# Operador ternario

El operador ternario nos va a permitir hacer una operación if else de una manera
muy sencilla utilizando una sola linea de código, este operador está compuesto
por tres partes

Definición

* a = Expresión a evaluar.
* b = Resultado si la condición se cumple.
* c = Resultado si la condición no se cumple.

Siendo de la forma:

`a ? b : c`

Un ejemplo de uso seria:

```js
let edad = 12;

edad > 18 ? console.log('Puede Votar') : console.log('No puede votar')
```

Se usa para asignar el valor a una variable

```js
let edad = 12;

let puedeVotar = edad > 18 ? 'Puede Votar' : 'No puede votar'

console.log(puedeVotar)
```

Es posible también anidar varias condiciones por medio de este operador:

```js
var a = 11;
var numberLiteral = a == 5 ? 'Five' :
                    a == 7 ? 'Seven' :
                    a == 11 ? 'Eleven' :
                    a == 15 ? 'Fifteen' :
                    'Other Number';
 
console.log( numberLiteral );
```

_Nota: No es recomendable tener más de 2 expresiones anidadas en un mismo
operador ternario, ya que la lectura y el mantenimiento de este tipo de
expresiones puede volverse complejo._

## Ejercicio
Crea una variable llamada `numero` y otra `esPar`. Haciendo uso del operador ternario asigna en la variable `esPar`, `verdadero`
(_true_) si `numero` es par o `falso` (_false_) si no lo es. Luego usa `console.log()` para imprimir la variable `esPar` a la consola.
