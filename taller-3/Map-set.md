# Metodo set

Establece un valor para `key` en el objecto `Map`. si la `key` no existe se agrega, si existe se actualiza

```js 
  const map = new Map();
  //agrega un nuevo par llave-valor
  map.set('mensaje', 'ibaguejs es genial');
  //actualizamos esa key
  map.set('mensaje', 'yo amo ibaguejs');
```

## Ejercicio
crea un objeto de tipo `Map` y agrega pares de llave-valor usando los siguientes tipos de datos, el valor puede ser cualquiera
  - string : `'texto'`
  - booleano : `true`  - `false`
  - numerico : 0 
  - Objecto : `{ mensaje:'soy un objeto' }`

  ## Ejemplo
  ```js
    const map = new Map()
    //con un dato tipo texto - string
    map.set('nombre', 'juanjs');

    console.log(map)
  ```
