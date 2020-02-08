# String charAt ()

Devuelve el carácter en el índice de cadena dado.

**Sintaxis**
character = str.charAt(index)

**Parámetros:** El único argumento para esta función es el índice en la cadena de donde se extraerá el carácter único. El rango de este índice está entre 0 y longitud - 1 , incluidos los límites. Si no se especifica ningún índice, el primer carácter de la cadena se devuelve ya que 0 es el índice predeterminado utilizado para esta función.

**Valores devueltos:** Esta función devuelve un solo carácter ubicado en el índice especificado como argumento de la función. Si el índice está fuera de rango, esta función devuelve una cadena vacía.

**Ejemplo:**
```js
var str = 'IbagueJs, comunidad Javascript de Ibagué';
console.log(str.charAt(2)); // a
```