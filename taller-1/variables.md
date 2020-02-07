# Variables

Una variable es una referencia a un valor. Podemos usar variables para representar cualquier valor del mundo real, algunos ejemplos de variables son:

```
color
distancia
edad
peso
nombre
```

Una forma de definir una variable es usando la palabra reservada `let`.

Por ejemplo:

```js
let example;
```

La variable anterior es **declarada**, pero no definida.

A continuación damos un ejemplo de cómo definir una variable, haciendo que referencie a un valor específico:

```js
const example = "some string";
```

Tienes la libertad de nombrar una variable a tu conveniencia, siguiendo dos reglas, la primera de forma obligatoria no puedes nombrar variables usando palabras reservadas del lenguaje JavaScript, algunas palabras reservadas son:

```js
const
let
var
return
void
```

Y la segunda regla que es opcional pero te ayudará a entender mejor tu código, es nombrar las variables con palabras que identifiquen el valor que almacena

```js
let edadDeLaPersona;
let nombre;
let cantidadDeHabitaciones;
let velocidadMaxima;
```

Nota que empieza con la palabra reservada `let` y usa el signo de igualdad entre en nombre de la variable y el valor que referencia. También podemos usar las palabras `var`, `const` incluso no usar ninguna de ellas, en cada uno de los casos nuestra variable tendrá un comportamiento diferente.

## Ejercicio

TBD
