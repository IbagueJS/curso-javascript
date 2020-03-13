# Metodo delete

Devuelve `true` si un elemento en el objeto `Map` existió y se eliminó, o `false` si el elemento no existe.

## Ejercio

Crear un objeto de tipo `Map`, agrega pares de llave-valor de los siguientes datos
 - nombre : julian
 - apellido : morales 
 - edad: 22
 - trabaja: true

en el objeto map elimina los pares de llave valor e imprime en un `console.log` si el par de llave valor fue eliminado

### ejemplo
```js
  const map = new Map()
  map.set('comunidad', 'ibaguejs')
  console.log(map.delete('comunidad'))
  // el resultado esperado es: true
  // true indica que fue removido exitosamente

  console.log(map.has('cominudad'))
  // false indica que no existe ya en el objecto map

  console.log(map.delete('comunidad'))
  // el resultado es false, dado que no existe no se puede eliminar

```