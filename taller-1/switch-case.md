# Switch Case

La declaración `switch` es un bloque condicional que permite evaluar diferentes
condiciones basadas en el valor de una variable otorgándole a cada condición un
comportamiento diferente. Esta declaración puede reemplazar múltiples
condicionales `if`.

Como funciona:

- La variable entre el paréntesis es evaluada una sola vez.
- Su valor es comparado con las expresiones declaradas en cada bloque `case`.
- Si existe una coincidencia exacta, la rutina de código dentro del bloque `case` es ejecutada.
- Si no existe coincidencia alguna, la rutina de código del bloque `default` es ejecutada.
- Una vez se ejecuta la rutina de código, la palabra reservada `break` rompe la ejecución del bloque `switch` y las comparaciones terminan.

La declaración `switch` se estructura de uno o varios bloques `case` y un bloque
opcional llamado `default`.

```js
const documentType = "CC";

switch (documentType) {
  case "CC":
  case "CE":
    console.log("Cédula de ciudadanía y extranjería");
    break;
  case "RC":
    console.log("Registro civil");
    break;
  case "TI":
    console.log("Tarjeta de identidad");
    break;
  default:
    console.log("Documentos de identidad");
    break;
}
```
Cabe resaltar que las expresiones usadas en la comparaciones pueden ser cadenas
de caracteres o números, sin embargo **No** se pueden evaluar distintos tipos de
datos en un mismo bloque `switch`.

## Ejercicio
Declara una variable llamada `day`. Haz que la variable `day` tenga como valor **6**.
Luego declara un bloque `switch` para comparar que día de la semana es, donde
**1** hace referencia al día **"Lunes"**. Dentro de cada bloque `case` utiliza
`console.log()` para indicar que día es y finalmente cuando la condición se
cumpla, imprime en la terminal "**Es sábado de IbaguéJS."**.
