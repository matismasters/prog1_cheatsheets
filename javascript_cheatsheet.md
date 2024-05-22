# Referencias rapidas de JavaScript

## Variables

```javascript
let variable = 1;
const constante = 2;

// Tipos de datos
let numero = 1;
let cadenaDeTexto = "Hola";
let booleano = true;
let array = [1, 2, 3];
let objeto = { nombre: "Juan", edad: 20 };

// Tipos de datos especiales
let nulo = null;
let indefinido = undefined;
```

## Operadores Aritméticos

```javascript
// Aritmeticos
let suma = 1 + 2;
let resta = 1 - 2;
let multiplicacion = 1 * 2;
let division = 1 / 2;
let modulo = 1 % 2;
```

## Operadores de Asignación

```javascript
// Asignacion
let asignacion = 1;
asignacion += 2; // a = a + 2;
asignacion -= 2; // a = a - 2;
asignacion *= 2; // a = a * 2;
asignacion /= 2; // a = a / 2;
asignacion %= 2; // a = a % 2;

// Incremento y Decremento
let incremento = 1;
incremento++; // incremento = incremento + 1;

let decremento = 1;
decremento--; // incremento = incremento - 1;
```

## Operadores de Comparación y Lógicos

```javascript
// Comparacion
1 == 2; // Igualdad
1 === 2; // Igualdad estricta 
1 != 2; // Diferente
1 !== 2; // Diferente estricto
1 > 2; // Mayor que
1 >= 2; // Mayor o igual que
2 < 2; // Menor que
2 <= 2; // Menor o igual que

// Logicos
// && AND: True si ambos son verdaderos
true && false;
// || OR: True si al menos uno es verdadero
true || false;
// ! NOT: Invierte el valor
!true;
```

## Condicionales

```javascript
// If y Else (Si y Sino)
let condicion = true;

if (condicion) {
    console.log("La condicion es verdadera");
}

if (condicion) {
    console.log("La condicion es verdadera");
} else {
    console.log("La condicion es falsa");
}

// Else If (Sino Si)
let numero = 1;

if (numero === 1) {
    console.log("El numero es 1");
} else if (numero === 2) {
    console.log("El numero es 2");
} else {
    console.log("El numero no es 1 ni 2");
}
```

## Ciclos

```javascript
// For
for (let i = 0; i < 5; i++) {
    console.log(i);
}

// While
let i = 0;
while (i < 5) {
    console.log(i);
    i++;
}

// Do While
let i = 0;
do {
    console.log(i);
    i++;
} while (i < 5);

```

## Ciclos con Arrays

```javascript
let arreglo = [1, 2, 3];

// Recorrer usando for con indice contador
for (let i = 0; i < arreglo.length; i++) {
    console.log(arreglo[i]);
}

// Recorrer usando for of
for (let elemento of arreglo) {
    console.log(elemento);
}

// Recorrer y llevar un contador
let contador = 0;
for (let elemento of arreglo) {
  if (elemento % 2 === 0) { // Contar pares
    contador++;
  }
}
```

## Funciones

```javascript
// Declaracion
function saludar() {
    console.log("Hola");
}

// Llamada
saludar();

// Con parametros
function saludar(nombre) {
    console.log("Hola " + nombre);
}

// Llamada pasando parametros
saludar("Juan");

// Con retorno
function sumar(a, b) {
    return a + b;
}

// Llamada con retorno
let resultado = sumar(1, 2);
```

## Array

```javascript
// Declaracion
let arreglo = [1, 2, 3];

// Acceso
let primerElemento = arreglo[0];

// Modificar
arreglo[0] = 4;

// Metodos
// Total de elementos
arreglo.length;
// Agrega al final
arreglo.push("elemento");
// Retornar y elimina el ultimo
arreglo.pop();
// Retornar y elimina el primero
arreglo.shift();
// Agrega al principio
arreglo.unshift("elemento");
// Elimina un elemento en la posicion 1
arreglo.splice(1, 1);
// Retorna un subarreglo con los elementos
// entre la posicion 1 hasta la 2
arreglo.slice(1, 2);
```

## String

```javascript
// Declaracion
let cadena = "Hola Mundo";

// Total de caracteres
cadena.length;
 // Convertir a mayusculas
cadena.toUpperCase();
 // Convertir a minusculas
cadena.toLowerCase();
 // Obtener el caracter en la posicion 0
cadena.charAt(0);
// Obtener la posicion de la palabra "Mundo"
cadena.indexOf("Mundo");
// Reemplazar "Mundo" por "Juan"
cadena.replace("Mundo", "Juan");
// Separar por espaciondo", "Juan");
cadena.split(" ");
// Retorna true si empieza con "Hola"
cadena.startsWith("Hola");
// Retorna true si termina con "Mundo";
cadena.endsWith("Mundo");
// Retorna true si contiene "und"
cadena.includes("und");
```

## Objetos

```javascript
// Declaracion
let objeto = {
  nombre: "Juan",
  edad: 20
};

// Declaracion en una linea
let objeto = { nombre: "Juan", edad: 20 };

// Acceso
let nombre = objeto.nombre;

// Modificar
objeto.nombre = "Pedro";

// Agregar
objeto.apellido = "Perez";

// Eliminar
delete objeto.edad;

```

## Clases

```javascript
// Declaracion
class Persona {
  // Constructor
  constructor(nombre, edad) {
    // Propiedades
    this.nombre = nombre;
    this.edad = edad;
  }

  // Metodos
  saludar() {
    console.log("Hola " + this.nombre);
  }
}

// Instanciar
let persona = new Persona("Juan", 20); 

// Llamar metodo
persona.saludar();

```