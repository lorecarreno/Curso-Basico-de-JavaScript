***Qué son las funciones en JavaScript***

Las funciones son bloques de código que solucionan un problema específico para ser reutilizados. Existen dos tipos de funciones: declarativas y expresivas.

**Qué son las funciones declarativas**

En JavaScript, las funciones declarativas se las declara con la palabra reservada *function*.

Cómo declarar una función declarativa
La declaración de una función declarativa está constituido por las siguientes partes:

- La palabra reservada function.

- El nombre de la función: el cual será guardado como referencia en memoria.

- Los parámetros: están envueltas en paréntesis (), son variables propias de la función y deberán utilizarse en el contenido. Hacen referencia a los argumentos en la invocación.

- El contenido: está envuelto por llaves {}, contendrá las líneas de código correspondientes a la lógica del problema.

- El valor retornado: es un único valor que devuelve la función cuando es llamada. Se lo especifica por la palabra reservada return. Si no existe, la función devolverá un valor undefined por defecto.

>// Declaración <br>
>function suma (a,b){ <br>
> return a + b <br>
>} <br>
>/*<br>
>function nombre (parámetros) { <br>
> contenido <br>
> return valor <br>
>} <br>
>*/ <br>

De esta manera, definimos la lógica de la función, pero no la estamos utilizando. Para generar los valores es necesario invocar la función en el código según sea necesario.

**Cómo invocar una función declarativa**

La invocación o llamada es la manera que utilizamos las funciones para utilizar el valor de retorno (return) según ciertos argumentos. La invocación de la función declarativa está constituido por dos partes:

- El nombre de la función especificada en la declaración.

- Los argumentos, son los valores para cada uno de parámetros de la función envueltos entre paréntesis.

>// Invocación <br>
>suma(2,3) <br>
>// nombre(argumentos) <br>

La invocación sirve para emplear una función con diferentes argumentos y guardarlos en una variable.

>var resultado1 = suma(2,3) <br>
>var resultado2 = suma(4,6) <br>
>var resultado3 = suma(10,12) <br>
> <br>
>console.log(resultado1) //5 <br>
>console.log(resultado2) //10 <br>
>console.log(resultado3) //22 <br>

También existen funciones que simplemente se invocan, pero debes tener en cuenta que retornan por defecto undefined.

>// Declaración <br>
>function saludar(nombre){ <br>
>    console.log("Hola " + nombre) <br>
>} <br>
>// Invocaciones <br>
>saludar("JavaScript") //"Hola JavaScript" <br>
>saludar("Platzi") // "Hola Platzi" <br>

**Plantillas literales**

También puedes utilizar las plantillas literales, una nueva característica del lenguaje para utilizar las variables dentro de ${variable} entre las tildes invertidas ( `` ),

>console.log(`Hola ${nombre}`) <br>

**Qué son las funciones expresivas o anónimas**

Las funciones expresivas o anónimas consisten en guardar la función en una variable. Tienen la misma declaración e invocación que las funciones declarativas. La diferencia consiste en no especificar un nombre en la función, sino que utiliza el nombre de la variable.

>// Declaración <br>
>var suma = function (a, b) { <br>
> return a + b <br>
>} <br>
>// Invocación <br>
>var resultado = suma(2, 2) <br>
> <br>
>console.log(resultado) //4 <br>


----------------------------------------------------------------
**Lecturas recomendadas**

[GitHub - degranda/jsBasico-: Ejemplos del curso de JS básico](https://github.com/degranda/jsBasico)
----------------------------------------------------------------
**Clases relacionadas**

[Qué es un objeto en JavaScript](https://platzi.com/clases/2332-javascript-poo/38619-que-es-un-objeto-en-javascript/)

[Cómo funciona el JavaScript Engine](https://platzi.com/clases/1642-javascript-profesional/22168-como-funciona-el-javascript-engine/)

[Curso Intermedio de Programación Orientada a Objetos en JavaScript](https://platzi.com/clases/2419-javascript-poo-intermedio/39811-como-funciona-la-memoria-en-javascript/)

[Curso de JavaScript Engine (V8) y el Navegador](https://platzi.com/clases/1798-javascript-navegador/25681-como-funciona-el-javascript-engine/)

