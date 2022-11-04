***¿Qué es un array?***


Un array es una estructura de datos que permite almacenar una serie de datos localizados por índices y separados por comas.

**Qué son los índices**

El índice es la forma en que accedemos a los elementos de los arrays. En JavaScript, los índices empiezan desde 0, es decir, la primera posición es el índice 0. Un array se inicia mediante la sintaxis de corchetes [] y es tipo de dato objeto.

>var array = [1,2,3,4] <br>

**Cómo acceder a los elementos del array**

Para acceder a los elementos del array se utiliza la siguiente estructura:

>array[índice]

Para saber la cantidad de elementos de un array se utiliza la propiedad length.

>var array = [1,2,3,4] <br>
>var longitud = array.length <br>
>console.log(longitud) // 4 <br>

Ten en cuenta que la posición del elemento es diferente al índice del mismo.

Entonces, para acceder a un elemento del array, únicamente podrás utilizar los índices desde el 0 hasta array.length -1. Si se accede a un índice que no existe, devolverá undefined.

>var nombres = ["Andres", "Ramiro", "Silvia"] <br>
> <br>
>nombres[0] // "Andres" <br>
>nombres[1] // "Ramiro" <br>
>nombres[2] // "Silvia" <br>
>nombres[3] // undefined <br>

**Qué es la mutabilidad en los arrays**

La mutabilidad hace referencia a la capacidad de una estructura de datos a cambiar. Esto permite cambiar los valores de los elementos de un array cuando accedemos a sus elementos mediante un índice.

Por ejemplo, cambiemos el segundo elemento con índice 1 al valor de “Platzi”:

>var nombres = ["Andres", "Ramiro", "Silvia"] <br>
>// Accedemos y mutamos el segundo elemento <br>
>nombres[1] = "Platzi" <br>
> <br>
>console.log(nombres) // ["Andres", "Platzi", "Silvia"] <br>

**Qué son los métodos de arrays**

Los métodos de arrays son funcionalidades extra. Es semejante a las funciones, pero se accede mediante la notación punto array.metodo(argumentos).

Existen métodos mutables, es decir, que cambian el array original. Estos métodos son:

- push
- unshift
- pop
- shift

**Cómo utilizar el método push**

El método push agrega uno o varios elementos al final del array original. El método recibe como argumento los valores a agregar. Retorna el número de elementos del array mutado.

>var array = [1,2,3] <br>
>array.push(4,5) <br>
>console.log(array) // [ 1, 2, 3, 4, 5 ] <br>

**Cómo utilizar el método unshift**

El método unshift agrega uno o varios elementos al inicio del array original. El método recibe como argumento los valores a agregar. Retorna el número de elementos del array mutado.

>var array = [3,4,5] <br>
>array.unshift(1,2) <br>
>console.log(array) // [ 1, 2, 3, 4, 5 ] <br>

**Cómo utilizar el método pop**

El método pop extrae el elemento del final del array original.

>var array = [1,2,3,4] <br>
>var lastElement = array.pop() <br>
>console.log(lastElement) // 4 <br>
>console.log(array) // [ 1, 2, 3 ] <br>

**Cómo utilizar el método shift**

El método shift extrae el elemento del inicio del array original.

>var array = [1,2,3,4] <br>
>var firstElement = array.shift() <br>
>console.log(firstElement) // 1 <br>
>console.log(array) // [ 2, 3, 4 ] <br>

**Cómo utilizar el método indexOf**

El método indexOf muestra el índice del elemento especificado como argumento.

>var array = [1,2,3,4] <br>
>var index = array.indexOf(2) <br>
>console.log(index) // 1 <br>

Si el elemento no se encuentra en el array, el método devuelve el valor -1.

>var array = [1,2,3,4] <br>
>var index = array.indexOf("hola") <br>
>console.log(index) // -1 <br>

----------------------------------------------------------------
**Lecturas recomendadas**

[GitHub - degranda/jsBasico-: Ejemplos del curso de JS básico](https://github.com/degranda/jsBasico)
