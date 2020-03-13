# Metodo keys

El método `keys()` devuelve un nuevo objeto `Iterator` que contiene las claves para cada elemento en el objeto `Map` en orden de inserción.

## Iterador en 5 minutos

En JavaScript un iterador es un objeto que define una secuencia y potencialmente un valor de retorno a su terminación.

Específicamente, un iterador es cualquier objeto que implemente el protocolo Iterator teniendo un método next() que devuelva un objeto con dos propiedades:

 - value: El siguiente valor en la secuencia de iteración.
 - done: Es un valor booleano si es `true` significa que ya ha finalizado, en caso contrario aun no ha terminado


## Ejemplo

```js 
  const map1 = new Map();

  map1.set('0', 'cero en string');
  map1.set(1, 'uno en numerico');

  //almacenamos el objeto iterador
  const iterator1 = map1.keys();

  console.log(iterator1.next().value);
  // expected output: "0"

  console.log(iterator1.next().value);
  // expected output: 1
```