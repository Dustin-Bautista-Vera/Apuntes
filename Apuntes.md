# Apuntes

## **_//alert("Estamos en el archivo EstructuraDeCiclo.js")_**

> //Estrctura de control for
for(let i=0; i<=10; i++){
    console.log("No Iteracion: "+ i);
}

> //Estructura de control while
let contador=1;

while (contador<10){
    console.log("No Iteracion: "+ contador);
    contador++;
}

> //Estructura de control do/while
let numero=1;
do{
    console.log(" [do/while] No Iteration: "+ numero);
    numero++;
} while(numero<10);

> //for in
let estudiante= {nombre:"Juan Perez", edad:18, calificacion: 70}

for(let propiedad in estudiante){
    console.log(propiedad + ":" + estudiante[propiedad]);
}

> //for...of
> //Este ciclo itera sopbre los valores de un objeto iterable (como un array)
`let mis_numeros=[10,20,30,40,50];`

for(let numero of mis_numeros){
    console.log(numero);
}
--- 

## **_//Calculadora de IMC_**

1. let Peso;
let Estatura;
    Peso= prompt("Ingrese su peso ");
    Estatura= prompt("Ingrese su estatura (En metros) ");

let value1= parseFloat(Peso);
let value2= parseFloat(Estatura*2);
let resultado= parseFloat(value1/value2);

 console.log("Su IMC es: " + (resultado));

    if(resultado<=18.5){
        console.log("Usted tiene desnutricion");
    } else if(resultado>=18.5 && resultado<=24.9){
        console.log("Su IMC es normal");
    } else if(resultado>=25 && resultado<=29.9){
        console.log("Usted tiene sobrepeso");
    } else if(resultado>=30 && resultado<=34.9){
        console.log("Usted tiene Obesidad Tipo 1");
    } else if(resultado>=35 && resultado<=39.9){
        console.log("Usted tiene Obesidad Tipo 2");
    } else if(resultado>40){
        console.log("Usted tiene Obesidad Tipo 3");
    }

1. //Estructuras con if, else, switch <>

let iEdad= 17;

// Solo if
    if(iEdad>=18){
        console.log("Eres un adulto y debes registrate en el SAT");
    }

// if/else
    if(iEdad>=18){
    console.log("Eres un adulto y debes registrate en el SAT");
    } else{
    console.log("Todavia no pagaras impuestos");
    }

1. //Operadores Aritmeticos
let a=10;
let b=3;
console.log(a+b);
console.log(a-b);
console.log(a*b);
console.log(a/b);
console.log(a%b);

1. //Operadores de Asignacion
let x=10;
x += 5;
x -= 2;
x *= 3;
x /= 3;
x %= 5;

1. - //Operadores de comparacion
- let c=5; let d='5';
- console.log(a==b); //true (Compara el valor pero no el signo)
- console.log(a===b); //false (Compara el valor pero no el signo)
- console.log(a!=b); //false
- console.log(a===b); //true (Compara el valor pero no el signo)
- console.log(a>b); //true (Compara el valor pero no el signo) <>
- console.log(a<=b); //true (Compara el valor pero no el signo)

1. //Operadores logicos
let e= true;
let f= false;

console.log(e && f); //false
console.log(e || f);
console.log(!f);

1. //Estructuras de control if/else anidado
> let Cargo= 200;

    if(Cargo>=100 && Cargo<=150){
        alert("Impuesto bajo");
    } else if(Cargo>=151 && Cargo<=200){
        alert("Impuesto medio");
    } else{
        alert("Revisar el tabulador");
    }
---

> **_//Asi se utilizan los comentarios de una sola linea en JAvaScript_**

```js
console.log("Biemvenidos al mundo de la programacion FrontEnd con JavaScript");

console.log("Esta en otra linea"+"Y se conecta con el +");

/*
Esto es un comentario de mas de una linea
*/

/*
    En javascript no existe 
*/

let estudiante= "Juan Perez";
let edad= 19;
let isEstudiante= true;
let calificacion= 92.2;

console.log("Estudiante" + estudiante);
console.log("Edad" + edad);
console.log("¿Estudia?" + isEstudiante);
console.log(typeof calificacion);
console.log('El promedio global del estudiante es $[calificacion]');
```