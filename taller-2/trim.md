# String trim()

La función str.trim() se utiliza para eliminar los espacios en blanco de ambos extremos de la cadena dada.

**Sintaxis:**

```js
str.trim ()
```

**Parámetros:** Esta función no toma ningún argumento.

**Valores devueltos:** Esta función devuelve una nueva cadena, sin ninguno de los espacios en blanco iniciales o finales.

**Ejemplo:**

```js
var str = "IbagueJs      ";
var st = str.trim();
console.log(st);
```

**Ejercicio:**

Genere una variable en la que almacene una contraseña (👀 no tu contraseña real, es solo un ejemplo), intencionalmente agrege algunos espacios en blanco al inicio y al final de la cadena, y haciendo uso de la funcion trim elimina dichos espacios en blanco, confirme que funciona imprimiendo el resultado en consola.