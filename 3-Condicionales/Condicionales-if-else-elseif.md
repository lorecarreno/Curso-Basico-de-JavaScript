***Condicionales: If, Else, else if***


Los condicionales son estructuras de control que te permiten evaluar diferentes expresiones y realizar determinadas acciones en JavasScript.

Cómo utilizar el condicional ifen JavaScript
Un condicional evalúa si una expresión o condición es verdadera. Por ejemplo, si mi edad es mayor o igual que 18, puedo conducir.

>if (edad >= 18){ <br>
>    console.log("Puedes conducir") <br>
>} <br>

La palabra reservada else evalúa cuando la expresión del if es falsa, pero no es obligatorio colocarlo. En el ejemplo anterior, la condición contraria del if es la edad menor que 18, entonces no puedes conducir.

>if (edad >= 18){ <br>
>    console.log("Puedes conducir") <br>
>} else { <br>
>    console.log("No puedes conducir") <br>
>} <br>

En otras palabras, si (if) una acción (expresión) es verdadera (true) hago una acción (bloques de código). En el caso contrario (else) efectúo otra acción.

Cómo anidar condicionales al programar

Has aprendido a usar un condicional, pero ¿y si tenemos varias condiciones? Entonces empleamos las palabras reservadas else if junto a la condición a ejecutar, puedes utilizar varias condiciones que necesites. Sin embargo, JavaScript evalúa la primera condición, luego a la segunda, y así sucesivamente. Esto es importante para ordenar las condiciones correctamente y no sobreescribirlas.

>if (condicion1){ <br>
>   // Bloque 1 <br>
>} else if (condicion2){ <br>
>    // Bloque 2 <br>
>} else if (condicion3){ <br>
>   // Bloque 3 <br>
>} else { <br>
>    // Bloque else <br>
>} <br>

Por ejemplo, un cliente solicita un descuento según el número de artículos que ha comprado, la tienda ofrece 3 descuentos: 10% si ha comprado más de 5 artículos, 15% si son más de 10 artículos, y todo por encima de 15 artículos recibe un 20% de descuento.

>var precio = 10 <br>
>if (articulos >= 5 && articulos < 10){ <br>
>   precio = precio *(1-0.10) <br>
>} else if (articulos >= 10 && articulos < 15){ <br>
>precio = precio* (1-0.15) <br>
>} else { <br>
>    precio = precio * (1-0.20) <br>
>} <br>

**Operador ternario**

El operador ternario consiste en evaluar si una expresión es verdadera o falsa. Parecido a un condicional, pero en una línea de código. Esto sirve para evaluar una condición de manera rápida. La estructura que sigue es la siguiente y se lee como: "La condición es verdadera (?), si es así ejecuta el “Bloque verdadero”, caso contrario (:), ejecuta el “Bloque falso”.

condicion ? Bloque verdadero : Bloque falso
Por ejemplo, guardemos en una variable un mensaje si un número es par o impar.

>function esPar(numero){ <br>
>    return numero % 2 === 0 ? "Es par" : "No es par" <br>
>} <br>

>esPar(2) // "Es par" <br>
>esPar(3) // "No es par" <br> 

**Ejercicio de condicionales**

Crea el juego de piedra, papel o tijera. Te dejo una pequeña ayuda para este reto:

Genera las variables correspondientes
Produce los condicionales que comparen tu resultado con el de la máquina u otra persona.
Encapsula los condicionales en una función que reciba las variables, compararlas y retornar un valor.


-------------------------------------------------------------------
**Lecturas recomendadas**

[Operador condicional (ternario) - JavaScript | MDN](https://developer.mozilla.org/es/docs/Web/JavaScript/Referencia/Operadores/Conditional_Operator)

[GitHub - degranda/jsBasico-: Ejemplos del curso de JS básico](https://github.com/degranda/jsBasico)
