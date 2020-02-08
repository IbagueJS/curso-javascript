# slice
Es una función muy útil, cuando queremos sacar una parte de un `String`, por ejemplo dividirlo a la mitad, o extraer los primeros 4 caracteres. Solo debemos decirle a la función desde cual posición desea iniciar y opcionalmente la posición final a extraer, al solo definir la posición inicial, `slice` irá hasta el último caracter de la cadena de texto.

> Ten en cuenta que el resultado no queda directamente sobre el `String` que estés manejando sino que devolverá el resultado para que lo almacenes en otra variable, por lo que la cadena de texto original, no se verá afectada.

```js
    let nombreCompleto = "Andrea Maria Suarez Alvarez"
    let nombres= nombreCompleto.slice(0,12)
    let apellidos=nombreCompleto.slice(13)
    
```

