# JavaScript

Variables, Funciones y Clases
Declaración de Variables y Arrow Functions
En JavaScript, puedes utilizar `let`, `var`, y `const` para declarar variables. `let` y `const` son formas modernas de declarar variables, mientras que `var` es más antiguo y tiene diferencias en cuanto al ámbito (scope).

```javascript
// Declaración de variables
let name = "world";
const pi = 3.14;

// Arrow function con parámetro opcional
let sayHello = (name = "world") => {
console.log("hello " + name);
};

sayHello(); // Imprime: "hello world"
sayHello("mario"); // Imprime: "hello mario"
```

# Clases en JavaScript
Las clases en JavaScript permiten definir objetos con métodos y propiedades. Aquí tienes un ejemplo de cómo declarar una clase, crear una instancia y utilizar métodos:

```javascript
// Declaración de una clase en JavaScript
class Persona {
constructor(nombre, edad) {
this.nombre = nombre;
this.edad = edad;
}

saludar() {
    console.log(\`Hola, soy \${this.nombre} y tengo \${this.edad} años.\`);
}
}

// Crear una instancia (objeto) de la clase Persona
let persona1 = new Persona("Juan", 30);

// Uso de un método de la clase
persona1.saludar(); // Imprime: "Hola, soy Juan y tengo 30 años."
```

# Módulos en JavaScript
Los módulos en JavaScript te permiten organizar tu código en archivos separados para modularizar y reutilizar funcionalidades. Para importar y exportar módulos, puedes utilizar `import` y `export`.

Ejemplo de exportación desde un archivo `modulo.js`:

```javascript
// modulo.js
export const suma = (a, b) => a + b;
export const resta = (a, b) => a - b;
```

Ejemplo de importación en otro archivo:

```javascript
// main.js
import { suma, resta } from './modulo.js';

console.log(suma(5, 3)); // Imprime: 8
console.log(resta(10, 4)); // Imprime: 6
```

# Estilo de Codificación en JavaScript
El estilo de codificación en JavaScript es importante para mantener un código limpio, legible y consistente. Algunas pautas comunes incluyen:

Usar nombres significativos para variables y funciones.
Seguir convenciones de capitalización (camelCase para variables y funciones, PascalCase para clases).
Usar indentación consistente (generalmente con espacios o tabs).
Utilizar comentarios claros y concisos.

