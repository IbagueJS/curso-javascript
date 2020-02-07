# Tipos de Datos

Las variables de JavaScript pueden contener muchos tipos de datos: números, cadenas, objetos y mucho más:

```js
var length = 12; // Number
var lastName = "Cristian"; // String
var x = { firstName: "John", lastName: "Doe" }; // Object
```

En la programación, tipos de datos es un concepto importante. Para poder operar
en variables, es importante saber algo sobre el tipo. Sin tipos de datos, un
ordenador no puede resolver con seguridad esto:

```js
var x = 12 + "IbaguéJS";
```

¿Tiene algún sentido para añadir "Volvo" a dieciséis? ¿Producirá un error o va a
producir un resultado?

JavaScript tratará el ejemplo anterior como:

```js
var x = "12" + "IbaguéJS";
```

JavaScript evalúa las expresiones de izquierda a derecha. Diferentes secuencias
pueden producir diferentes resultados:

```js
var x = 12 + 2 + "IbaguéJS";
var x = "IbaguéJS" + 12 + 2;
```

## Tipos dinámicos

JavaScript tiene tipos dinámicos. Esto significa que la misma variable puede ser
utilizado para contener diferentes tipos de datos:

```js
var x; // Now x is undefined
x = 5; // Now x is a Number
x = "John"; // Now x is a String
```

Un valor de datos primitivo es un solo valor de datos simple sin propiedades y
métodos adicionales.

El operador `typeof` puede devolver uno de estos tipos primitivos:

- string
- number
- boolean
- undefined

### Strings

Una cadena (o una cadena de texto) es una serie de caracteres o letras como
"IbaguéJS".

Las cadenas se escriben con comillas. Puede usar comillas simples o dobles:

```js
var meet1 = "IbaguéJS";
var meet2 = "IbaguéJS";
```

### Number

JavaScript tiene sólo un tipo de números. Los números se pueden escribir con o
sin decimales:

```js
var x1 = 34.0; // Written with decimals
var x2 = 34; // Written without decimals
var y = 123e5; // 12300000
var z = 123e-5; // 0.00123
```

### Boolean

Booleanos sólo puede tener dos valores: `true` o `false`.

```js
var x = 5;
var y = 5;
var z = 6;
(x == y)(
  // Returns true
  x == z
); // Returns false
```

### Arrays

Matrices de JavaScript se escriben con corchetes `[]`. Elementos de matriz están
separados por comas.

```js
var ibaguéjs = ["Andres", "Jose", "Giovanny", "Yeison", "Diego"];
```

Los índices de los array inician en cero, lo que significa que el primer
elemento es [0], el segundo es [1], y así sucesivamente.

### Objects

Objetos JavaScript se escriben con llaves `{}`.

Propiedades del objeto se escriben como nombre: pares de valores, separados por
comas.

```js
var ibaguéjsobj = {
  firstName: "Ibag",
  lastName: "ueJS",
  age: 1,
  color: "amarillo"
};
```

## undefined

En JavaScript, una variable sin un valor, tiene el valor undefined. El tipo es
también undefined.

```js
var car;
```

Un valor vacío no tiene nada que ver con undefined.

```js
var car = "";
```

## null

En JavaScript nulls "nada". Se supone que es algo que no existe. Por desgracia,
en JavaScript, el tipo de datos nulls un objeto.

```js
var t = "IbaguéJS";
t = null;
```

## Ejercicio

Use los comentarios para describir el tipo de datos correcto de las siguientes
variables:

```js
var longitud = 16; //
var lastName = "Johnson"; //
var x = {
  nombre: "Juan",
  Apellido: "Doe"
}; //
x = null; //
```

Use `typeof` para comprobar sus respuestas luego de haberlas puesto en cada uno
de los comentarios.
