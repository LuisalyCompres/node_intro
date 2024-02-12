# Introducción a Node.js
1. ### ¿Qué es Node.js?
Es un entorno de ejecución de JavaScript del lado del servidor que permite a los desarrolladores utilizar JavaScript para escribir código que se ejecuta en el servidor en lugar de en el navegador. 

2. ### Uso de Javascript necesario para usar Node.js:
- **Lexical Structure:** Se refiere a la sintaxis y la estructura básica del código JavaScript, incluyendo reglas para la declaración de variables, funciones, operadores, comentarios, etc. Es fundamental entender la estructura léxica para escribir código JavaScript válido.
```javascript
var x = 10;
function saludar() {
    console.log("Hola mundo!");
}
var suma = 5 + 3;
```
- **Expressions:** Las expresiones son unidades de código que producen un valor. Pueden ser tan simples como una variable o tan complejas como una llamada a una función. Es importante comprender cómo construir y evaluar expresiones en JavaScript.
```javascript
var resultado = 5 * (2 + 3);
var miFuncion = function() {
    return "Hola";
};
```
- **Data Types:** JavaScript tiene varios tipos de datos, como números, cadenas, booleanos, objetos y funciones. Es importante entender cómo trabajar con estos tipos de datos y cómo JavaScript los trata en diferentes contextos.
```javascript
var numero = 10;
var texto = "Hola";
var esVerdadero = true;
var persona = { nombre: "Maria", edad: 21 };
```
- **Classes:** A partir de ECMAScript 2015 (ES6), JavaScript introdujo la sintaxis de clases para permitir la programación orientada a objetos más fácil y clara. Las clases en JavaScript son sintácticamente similares a las clases en otros lenguajes de programación orientados a objetos.
```javascript
class Persona {
    constructor(nombre) {
        this.nombre = nombre;
    }
    saludar() {
        console.log("Hola, soy " + this.nombre);
    }
}
var persona = new Persona("Juan");
persona.saludar();
```
- **Variables:** En JavaScript, las variables se utilizan para almacenar valores. 
```javascript
var x = 10;
let y = 20;
const PI = 3.1416;
```
- **Functions:** Las funciones son bloques de código reutilizables que realizan una tarea específica. 
```javascript
function sumar(a, b) {
    return a + b;
}
var restar = function(a, b) {
    return a - b;
};
```
- **this operator:** El operador this se refiere al objeto en el contexto actual de ejecución. En Node.js, entender cómo this se comporta en diferentes contextos es importante, especialmente al trabajar con objetos y funciones.
```javascript
var persona = {
    nombre: "Maria",
    saludar: function() {
        console.log("Hola, soy " + this.nombre);
    }
};
persona.saludar();
```
- **Arrow Functions:** Las funciones de flecha son una característica introducida en ECMAScript 2015 (ES6) que proporciona una sintaxis más concisa para definir funciones en JavaScript. 
```javascript
var sumar = (a, b) => a + b;
console.log(sumar(5, 3));
```
- **Loops:** Los bucles se utilizan para repetir una serie de instrucciones hasta que se cumple una condición específica. 
```javascript
for (let i = 0; i < 5; i++) {
    console.log(i);
}
let j = 0;
while (j < 5) {
    console.log(j);
    j++;
}
```
- **Scopes:** El alcance de una variable se refiere a la parte del código donde esa variable es accesible. 
```javascript
var x = 10; 
function miFuncion() {
    var y = 20; 
    console.log(x); 
    console.log(y); 
}
miFuncion();
console.log(x); 
console.log(y);
```
- **Arrays:** Los arrays son estructuras de datos que permiten almacenar múltiples valores en una sola variable. 
```javascript
var numeros = [1, 2, 3, 4, 5];
console.log(numeros.length);
console.log(numeros[0]);
```
- **Template Literals:** Las template literals son una característica introducida en ECMAScript 2015 (ES6) que permite la interpolación de variables dentro de cadenas de texto de una manera más legible y conveniente. Son útiles para crear cadenas de texto dinámicas en Node.js.
```javascript
var nombre = "Juan";
var mensaje = `Hola, mi nombre es ${nombre}`;
console.log(mensaje);
```
- **Strict Mode:** El modo estricto (strict mode) es una característica de JavaScript que permite optar por una versión más restringida y segura del lenguaje. 
"use strict";

- **ECMAScript 2015 (ES6) and beyond:** ECMAScript 2015, también conocido como ES6, introdujo muchas nuevas características y mejoras en JavaScript, como las clases, las arrow functions, los template literals, y más. 
```javascript
class Persona {
    constructor(nombre) {
        this.nombre = nombre;
    }
    saludar = () => {
        console.log(`Hola, soy ${this.nombre}`);
    };
}
var persona = new Persona("Juan");
persona.saludar();
```
# Asynchronous Programming
Permite ejecutar operaciones sin bloquear el hilo de ejecución principal. Los callbacks son funciones que se ejecutan después de completarse una operación asincrónica. ***Sus conceptos principales son los siguientes:***

1. **Timers:** Funciones que permiten retrasar la ejecución de código en un tiempo determinado o a intervalos regulares.
2. **Promises:** Objetos que representan el resultado (éxito o fracaso) de una operación asincrónica, permitiendo un manejo más limpio y estructurado del código.
3. **Async and Await:** Características introducidas en ES8 para escribir código asincrónico de manera más legible y sencilla. ***async*** declara funciones asincrónicas y ***await*** pausa la ejecución hasta que una promesa se resuelve.
4. **Closures:** Funciones que conservan el contexto léxico en el que fueron creadas, útiles para capturar el estado de variables incluso después de que su ámbito original haya terminado.
5. **The Event Loop:** Mecanismo que controla la ejecución de operaciones en entornos asincrónicos como navegadores y Node.js, asegurando que el programa no se bloquee y que las operaciones se ejecuten en el orden correcto.







