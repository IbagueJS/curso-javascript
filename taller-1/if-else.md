# If & Else
Los bloques condicionales son utilizados, partiendo de una condición booleana
específica, alterar el control de flujo de un programa.

Un bloque condicional se parece a lo siguiente:

```js
if (n > 1) {
  console.log('la variable n es mayor a 1.')
} else {
  console.log('la variable n es menor o igual a 1.')
}
```

Dentro de los paréntesis debes ingresar una sentencia lógica, significa que
deberá ser verdadera (true) o falsa (false). Utilice la ifdeclaración para
especificar un bloque de código JavaScript que se ejecutará si una condición es
verdadera.

El *else* block es opcional y contiene el código que será ejecutado si la
sentencia lógica dentro de los paréntesis es falsa. Utilice la *else if*
declaración para especificar una nueva condición si la primera condición es
falsa.

## Ejercicio
Declara una variabe llamada `fruit`. Haz la variable `fruit` referenciar a la cadena de caracteres **"orange"**.

Luego utiliza `console.log()` para imprimir a la terminal "**The fruit name has
more than five characters."** si el length de la variable `fruit` es mayor a
cinco. Imprime "**The fruit name has five characters or less.**" de lo contrario.

