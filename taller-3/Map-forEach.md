# Metodo forEach

El método `forEach()` ejecuta una función proporcionada una vez por cada par llave-valor en el objeto `Map`, en el orden de inserción.

## Ejemplo
```js
  // esta funcion imprimira los pares llave-valor

  const map = new Map()

  map.set('uno', 1)
  map.set('dos', 2)
  map.set('tres', 3)

  function logMapElements(value, key) {
    console.log(`llave ${key}: valor ${value}`);
  }

  // el metodo for each recibe como para metro la funcion logMapElements y por cada par llave-valor que se encuentre en el map
  map.forEach(logMapElements);

  // salida esperada: "llave uno : valor 1"
  // expected output: "llave dos : valor 2"
  // expected output: "llave tres : valor 3"
```

