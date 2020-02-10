# push

Para insertar elementos en un array podemos asignar un valor al array en un
determinado índice el dato queda almacenado y eventualmente el atributo `length`
modificado.

Esta sintaxis tenemos que tener cuidado como variamos el subíndice para no dejar
componentes vacías si queremos implementar un array denso.

```
var array = ["Casa", "Avion", "Moto", "Carro"];
array.push("Patineta")
```

El método push depende de la propiedad `length` para decidir donde empezar a
insertar los valores dados. Si el valor de la propiedad `length` no puede ser
convertido en numérico, el índice 0 es usado. Esto permite la posibilidad de que
la propiedad `length` sea inexistente, y en este caso length será creado.

## Ejercicio

Use el array de la explicacion, con el metodo `push()` agregue 5 elementos
adicionales e imprima el resultado con `console.log()`.
