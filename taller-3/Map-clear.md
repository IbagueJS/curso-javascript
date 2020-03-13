# Metodo clear

Elimina todos los pares llave-valor del objeto `Map`.

## Ejemplo
```js
  const map = new Map()
  map.set('nombre', 'ibaguejs')
  map.set('edad', 1)
  map.set('es grandioso ibaguejs', true)

  console.log(map)

  //limpiamos y/o borramos los pares de llave valor del mapa
  map.clear()

  console.log(map)
``` 

## Ejercicio

Crea un objecto de tipo `Map` con n pares de llave-valor, luego limpiar el objeto map 