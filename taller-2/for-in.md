# Ciclo for in

La sentencia _for in_ realiza un bucle a través de las llaves de un objecto _{nombre: 'juan', edad: 22, comunidad:'ibaguejs' }_ donde 
nombre es la llave y el _'juan'_ es el valor


un bucle _for in_ se parece a lo siguiente:

```js
var persona = {nombre: 'juan', edad: 22, comunidad:'ibaguejs' }
for (var llave in persona) {
   console.log(llave);
   //para acceder al valor de la llave sobre el objecto
   console.log(persona[llave])
}
```

Recuerda que la sentencia _for in_ solo funciona sobre objetos 

## Ejercicio

Crea un objeto para iterar sobre sus llaves y utiliza `console.log()` para imprimir en la terminal la llave y el valor que tiene es llave en el objeto


