# pop

Este método elimina el último elemento del array. Automáticamente cuando
llamamos al método push el valor que le pasamos en el parámetro se almacena en
el array y se incrementa el atributo length.

```
var frutas = ["Banana", "Orange", "Apple", "Mango"];
frutas.pop();
```

`pop` es intencionadamente genérico; este método puede ser `called` o `applied`
en objectos similares a un array. En objetos que no contengan una propiedad
`length`, que refleje su forma en una serie de propiedades numéricas consecutivas
en base cero, puede no comportarse de manera significativa.

Si se llama a `pop()` en un array vacío, devuelve `undefined`.

## Ejercicio

Use el array de la explicacion, con el metodo `pop()` deje el array con solo
item `"Banana"` e imprima el resultado.
