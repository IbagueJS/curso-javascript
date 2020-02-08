# while

Ciclo que ejecturá un bloque de código siempre cuando la condición especificada sea `true`

**Sintaxis:**
```js
    while (condicion) {
      // bloque de código a ejecutarxs
    }
```
**Ejemplo:**
```js
    var dias = 1;
    while (dias <= 365) {
      console.log("Día " + dias);
      dias = dias + 1;
    }
```
El ejemplo anterior primero, declara una variable llamada `dias`y la inicializa con el valor `1`, posteriormente describe la sintaxis de un ciclo `while`, cuya condición consite en validar si `dias` es menor o igual a 365, si esta condicion se cumple se ejecturá el bloque de codigo que se encuentra dentro de las llaves **n** cantidad de veces hasta que esa condición se deje de cumplir.

Por otra parte, el bloque de código que se encuentra dentro del `while` se encarga de imprimir en consola el valor que tiene la variable `dias` durante cada repetición del ciclo, además, posteriormente se encarga de asignarle a la variable `dias` el valor que tiene en ese instante más uno.

_Es importe tener en cuenta que en el bloque de codigo que se encuentra dentro del `while`, se debe realizar una modificación de las variables que se validan en la **condición** del `while` (en el ejemplo anterior se realizaba esto incrementando `dias` una unidad por cada ciclo), ya que si la condición nunca se deja de cumplir el bloque de código se ejecutará hasta el fin de los tiempos o hasta que se desborde la memoria de tu computador, lo  que pase primero_  ¯\\_(ツ)_/¯

## Ejercicio

Usa el ciclo `While` para imprimir en consola los números del 100 al 0. 

_Recuerda que puedes utilizar `console.log()` para imprimir en consola_
