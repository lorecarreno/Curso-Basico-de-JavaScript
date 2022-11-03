***Coerción***

La coerción consiste en transformar de un tipo de dato a otro de una variable. Existen dos tipos de coerción: implícita y explícita.

**Qué es la coerción implícita**

La coerción implícita consiste en la transformación de tipos mediante la ayuda de JavaScript. Esto ocurre en operaciones de diferentes tipos, ya que es un lenguaje débil y dinámicamente tipado.

Al momento de compilar el código, el motor de JavaScript, si encuentra alguna incoherencia (una suma de un número con un string), el motor lo interpreta a su manera y arroja un valor que puede ser erróneo.

Algunos de los ejemplos de coerción implícita son los siguientes:

>4 + "7" // 47 <br>
>4 * "7" // 28 <br>
>2 + true // 3 <br>
>false - 3 // -3 <br>
>!3 // false <br>

Para evitar esto realiza la coerción explícita para manejar tipos de datos iguales antes de realizar cualquier operación.

**Qué es la coerción explícita**

La coerción explícita es la transformación de tipos de datos que controlamos el resultado. Para realizar estas transformaciones utiliza las funciones Number(), String() y Boolean(), para convertir a tipo número, string y lógico, respectivamente.

>Number("47") // 47 <br>
>String(51) // "51" <br>
>Boolean(1) // true <br>

Puedes utilizar la palabra reservada typeof para comprobar el tipo de dato transformado.

>Number("47") // 'number' <br>
>String(51) // 'string' <br>
>Boolean(1) // 'boolean' <br>

----------------------------------------------------------------
**Lecturas recomendadas**

[GitHub - degranda/jsBasico-: Ejemplos del curso de JS básico](https://github.com/degranda/jsBasico)


