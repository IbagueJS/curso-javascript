# Operadores

Un operador es un elemento que define una operación a realizar sobre una variable, un valor o varios de ellos. Hay diferentes tipos, unos mayormente usados que otros, veámoslos.

## Operadores de asignación

Asignan a la variable de la izquierda un valor basado en la expresión de la derecha, el operador de asignación básico es el igual (=).

Por ejemplo si queremos asignar el valor **3** a la variable **variable1** sería:

```js
variable1 = 3;
```

O si queremos asignar el valor de **variable1** a **variable2** sería:

```js
variable2 = variable1;
```

También podemos asignar datos diferentes a números.
Si queremos asignar el texto "Hola IbaguéJS" a la variable **varTexto** sería:

```js
varTexto = "Hola IbaguéJS";
```

Al ser el `"igual" ( = )` el operador de asignación básico, todos los demás operadores de asignación son una combinación entre él y alguna de las operaciones que veremos seguidamente.

#### Operadores de asignación

| Nombre                                              |    Uso    |
| --------------------------------------------------- | :-------: |
| Asignación                                          |   x = y   |
| Asignación de adición                               |  x += y   |
| Asignación de sustracción                           |  x -= y   |
| Asignación de multiplicación                        |  x \*= y  |
| Asignación de división                              |  x /= y   |
| Asignación de residuo                               |  x %= y   |
| Asignación de exponenciación a la izquierda         | x \*\*= y |
| Asignación de desplazamiento a la derecha           |  x <<= y  |
| Asignación de desplazamiento a la derecha sin signo |  x >>= y  |
| Asignación de desplazamiento                        | x >>>= y  |
| Asignación AND binaria                              |  x &= y   |
| Asignación XOR binaria                              |  x ^= y   |
| Asignación OR binaria                               |     x     | = y |

## Operadores de comparación

Comparan dos valores y devuelven un valor lógico (`booleano`) basado en si la comparación es verdadera (`true`) o falsa (`false`).
Tomemos como ejemplo dos variables,

```js
var1 = 3;
var2 = 4;
```

#### Igualdad (==)

Devuelve `true` si ambos operandos son iguales.

```js
3 == var1;
"3" == var1;
3 == "3";
```

#### Desigualdad (!=)

Devuelve `true` si ambos operandos no son iguales.

```js
var1 != 4;
var2 != "3";
```

#### Mayor que (>)

Devuelve `true` si el operando de la izquierda es mayor que el operando de la derecha.

```js
var2 > var1;
"12" > 2;
```

#### Mayor o igual que (>=)

Devuelve `true` si el operando de la izquierda es mayor o igual que el operando de la derecha.

```js
var2 >= var1;
var1 >= 3;
```

#### Menor que (<)

Devuelve `true` si el operando de la izquierda es menor que el operando de la derecha.

```js
var1 < var2;
"2" < 12;
```

#### Menor o igual que (<=)

Devuelve `true` si el operando de la izquierda es menor o igual que el operando de la derecha.

```js
var1 <= var2;
var2 <= 5;
```

> Todos los ejemplos anteriores retornan `true`, es tu turno de escribir comparaciones que retornen `false`.

Otros operadores de comparación son los de `estrictamente iguales ( === )` y `estrictamente desiguales (!==)`.

## Operadores aritméticos

Como en otros lenguajes de programación JavaScript nos permite realizar operaciones aritméticas, contando principalmente con las operaciones básicas:
`+`, suma
`-`, resta
`*`, multiplicación
`/`, división

Ejemplo:

```js
1 + 2; // 3
3 - 5; // -2
1 / 2; // 0.5
4 * 3; // 12
```

Y con variables también

```js
// Asignamos valores a las variables
var1 = 5;
var2 = 10;
// Operamos las variables
var1 + var2; // 15
var2 / var1; // 2
```

También podemos `asignar` el resultado de cualquier operación (tanto aritmética, como las demás) a una variable.

```js
var1 = 100;
var2 = 200;
resultado = var1 * var2;
```

Otros operadores aritméticos muy útiles son:

#### Residuo (%)

Devuelve el residuo de una división.

```js
5 % 2; // 1
```

#### Incremento (++)

Incrementa una vez al operando (le suma 1).

```js
var1 = 3;
var1++;
//ahora var1 es 4
var1++;
//ahora var1 es 5
var1++;
//ahora var1 es 6
```

#### Decremento (--)

Decrementa una vez al operando (le resta 1).

```js
var1 = 3;
var1--;
//ahora var1 es 2
var1--;
//ahora var1 es 1
var1--;
//ahora var1 es 0
```

> Reto: Los operadores de incremento y decremento se pueden usar como prefijo o sufijo al valor a operar, tu reto es identificar la diferencia:

```js
var1 = 3;
var2 = 3;
//Encuentra la diferencia entre las siguientes dos líneas:
varM = var1++;
varN = ++var2;
```

> Es de notar que los operadores de incremento y decremento, realizan también la operación de asignación sobre la variable.

#### Potencia (\*\*)

Eleva un valor a una potencia dada

```js
5 ** 2; // 25, 5 es la base y 2 el exponente
var1 = 7;
varCuadrado = var1 ** 2; // 49
```

## Operadores lógicos

Evalúa dos expresiones y retorna un valor lógico (`booleano`). Son principalmente utilizados con valores `booleanos (true), (false)`.

#### AND (&&)

Devuelve `true` si ambos operandos son `true`, en caso contrario devuelve `false`

```js
var a1 = true && true; // t && t devuelve true
var a2 = true && false; // t && f devuelve false
var a3 = false && true; // f && t devuelve false
var a4 = false && 3 == 4; // f && f devuelve false
```

#### OR (||)

Devuelve true si alguno de los operandos es `true`, o `false` si ambos son `false`.

```js
var o1 = true || true; // t || t devuelve true
var o2 = false || true; // f || t devuelve true
var o3 = true || false; // t || f devuelve true
var o4 = false || 3 == 4; // f || f devuelve false
```

#### NOT (!)

Devuelve el valor lógico contrario al actual.

```js
var n1 = !true; // !t devuelve false
var n2 = !false; // !f devuelve true
```

> Tip: Se utilizan las tablas de verdad como herramienta para facilitar la comprensión de los operadores lógicos.

> Nota: Los operadores lógicos son usados también con valores que no son `booleanos`, y su comprensión es un poco diferente, la veremos más adelante.

## Combinando operadores

En una sola línea podemos combinar diferentes operadores (¡con algunas reglas claro está!),

Ejemplo,

```js
var var1 = 5;
var var2 = 10;
var resultadoMatematico = 2 + var1 * var2 - 5 ** 3 / var2;

var resultadoLogico = var1 > var2 || var2 >= 5;
```

Para agrupar operaciones no dudes en utilizar los paréntesis, te facilitará las cosas

```js
var var1 = 5;
var var2 = 10;
var resultadoMatematico = (2 + var1 * var2 - 5 ** 3) / var2;
var resultadoLogico = (var1 > var2 || var2 >= 5) && !(var1 == 3 || var2 != 8);
```

> Tip: Escribir operaciones en programación es bastante similar a como lo hacemos en algebra, así que déjalo fluir.

## Otros operadores

- Operador condicional (ternario)
- Operadores Bit a bit
- Operador coma
- Operadores unarios
- Operadores relacionales

Más adelante podremos profundizar en otros operadores y algunos `trucos` al usar operadores.

## Ejercicios

Declara dos variables asignandoles un número a cada una, luego en una tercer variable almacena el valor de comparar si la primer variable es menor que la segunda.

Usando las mismas variables, realiza las 4 operaciones básicas entre ellas y muestralas en consola.

A la segunda variable que usaste usa el operador de incremento, 2 veces y muestra el valor en consola.

