***Valores: Truthy y Falsy***

Los valores truthy y falsy son valores verdaderos y falsos cuando se realiza una coerción de cualquier tipo a booleano, respectivamente. Esto es importante para manejar condicionales, ya que una estructura condicional evalúa si un valor es verdadero o falso en un contexto booleano.

**Qué son los valores falsy**

Un valor falsy es aquel que es falso en un contexto booleano, estos son: 0, "" (string vacío), false, NaN, undefined o null.

>// Coersión explícita <br>
>Boolean(0) // false <br>
>Boolean("") // false <br>
>Boolean(null) // false <br>
>Boolean(undefined) // false <br>
>Boolean(NaN) // false <br>
>Boolean(false) // false <br>

También puedes realizar una coerción implícita con el operador de negación (!), pero solo es para que la conozcas, no es recomendable.

>// Coersión implícita (no la uses)
>!!0 // false <br>
>!!"" // false <br>
>!!null // false <br>
>!!undefined // false <br>
>!!NaN // false <br>
>!!false // false <br>

**Qué son los valores truthy**

Un valor truthy es aquel que es verdadero en un contexto booleano, son todos los valores que no sean falsy, que especificamos en la anterior sección.

// Coersión explícita <br>
Boolean(12) // true <br>
Boolean("hola") // true <br>
Boolean(true) // true <br>
Boolean([1, 2, 3]) // true <br>
Boolean(function hola() {}) // true <br>
Boolean({ a: 1, b: 2 }) // true <br>

Cabe recalcar que en JavaScript todo valor que no sea falsy es truthy incluyendo las estructuras vacías de array y objetos.

Boolean([]) // true <br>
Boolean({}) // true <br>

----------------------------------------------------------------

**Lecturas recomendadas**

[GitHub - degranda/jsBasico-: Ejemplos del curso de JS básico](https://github.com/degranda/jsBasico)
