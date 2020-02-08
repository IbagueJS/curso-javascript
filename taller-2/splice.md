# splice

El método _splice_ adiciona o remueve ítems de un arreglo y retorna el/los ítem(s) removidos. Los elementos se añaden o remueven dado un _index_ inicial y de manera opcional _howmany_ se indican la cantidad de elementos a remover y la cantidad de _...items_ a añadir.

Adicionar nuevos elementos sin remover ningún valor del arreglo original

```js
var metodos = ["slice", "join", "concat", "pop"];
metodos.splice(2, 0, "length", "push");
```

Adicionar nuevos elementos removiendo un valor del arreglo original

```js
var metodos = ["slice", "join", "concat", "pop"];
metodos.splice(2, 1, "length", "push");
```

Remover valores del arreglo original sin añadir nuevos elementos

```js
var metodos = ["slice", "join", "concat", "pop"];
metodos.splice(2, 2);
```

La sintaxis del método _splice_ es la siguiente:

`array.splice(index, howmany, item1, ..., itemx)`

_Nota: Si el parámetro "howmany" es 0 no se remueve ningún valor del arreglo. El arreglo original es modificado_

## Ejercicio

Cree un arreglo con 8 nombres de frutas, remueva el elemento en la posición 3, después añada 2 nuevas frutas desde la posición 4 en adelante. Para finalizar añada una última fruta sin remover ningún elemento del arreglo, utilice `console.log()` para imprimir los valores que actualmente tiene el arreglo.
