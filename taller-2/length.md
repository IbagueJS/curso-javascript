# length

Supongamos que en un formulario de registro de usuarios, queremos validar si el nombre de usuario escogido cumple ciertas caracteristicas, entre las cuales está, que tenga una longitud de al menos 5 caracteres, un usuario podría escoger cualquier nombre como el del siguiente ejemplo:

```js
    let usuario = "jz";
```
La propiedad `length` nos permite conocer el tamaño o longitud del `String` en cuestión para luego tomar decisiones como informar al usuario que no se permite ese tamaño de variable, o en caso de ser un tamaño permitido continuar con el registro.

```js
    let usuario = "jz";
    
    if (usuario.length < 5 ){ //La longitud del String será de 2 caracteres
        console.log("No se permite un nombre de usuario de menos de 5 carácteres, escoja otro")
    }else{
        console.log("Puede continuar con el registro")
    }
```

## Ejercicio

Crea dos variables y almacena tu nombre y el de un compañero, luego imprime en pantalla el nombre con mayor cantidad de caracteres. (Recuerda usar el condicional `if`)


