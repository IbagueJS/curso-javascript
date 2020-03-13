# Metodo get

Devuelve el valor asociado a la key, o `undefined` si no se encuentra en el mapa.

```js 
  // crear un nuevo mapa  
  const map = new Map()
  // asignar un nuevo par llave-valor
  map.set('nombre', 'juanjs')
  // obtener ese nuevo valor
  console.log(map.get('nombre'))
  //obtener un valor con una llave que no existe en el mapa
  console.log(map.get('edad'))
  //como resultado dara undefined
```

## Ejercicio 
crea el siguiente objecto `Map` y determina con el operador _typeof_ que tipo de dato esta almacenando la llave

```js
  const mapa = new Map()
  map.set('nombre', 'ibagues')
  map.set('edad', 1)
  map.set('es grandioso ibaguejs', true)
  map.set('miembro', { patrocinadores: 'SENA', lugar: 'Picaleña' })
```






