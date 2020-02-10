# shift

El método `shift()` elimina el primer elemento del array y lo retorna. Este método
modifica la longitud del array.

El método `shift` elimina el elemento en el índice cero y desplaza los valores
consecutivos hacia abajo, devolviendo el valor eliminado. Si la propiedad
`length` es 0, devuelve `undefined`.

```
var miPescado = [1, 2, 3, 'ángel', 'payaso', 'mandarín', 'cirujano'];
miPescado.shift()
```

## Ejercicio

Use el array de la explicacion, con el metodo `shift()` deje el array con solo
items de tipo texto e imprima el resultado.
