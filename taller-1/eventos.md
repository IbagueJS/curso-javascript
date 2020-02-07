# Eventos

Un evento HTML puede ser algo que el navegador lo hace, o algo que un usuario
hace.

Estos son algunos ejemplos de eventos de HTML:

- Una página web HTML tiene terminado de cargar
- Un campo de entrada HTML fue cambiado
- Se hace clic en un botón de HTML

A menudo, cuando los eventos ocurren, es posible que desee hacer algo.

JavaScript permite ejecutar código cuando se detectan eventos. HTML permite
atributos de control de eventos, con código JavaScript, que se añade a los
elementos HTML.

```html
<button event="some JavaScript"></button>
```

En el siguiente ejemplo, el código cambia el contenido de su propio elemento
(usando this.innerHTML):

```html
<button onclick="this.innerHTML = Date()">The time is?</button>
```

## Ejercicio

El elemento <button> debe hacer algo cuando alguien hace clic en él. ¡Intenta
arreglarlo!

```html
<button xxxxxx="alert('hola')">Haga clic en aquí.</button>
```
