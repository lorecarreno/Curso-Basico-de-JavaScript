Switch


La **estructura switch es otra manera de evaluar condiciones, la diferencia con if es que las condiciones deben ser iguales a un caso o algo específico.

**Cómo utilizar el condicional switch**
Colocamos la palabra reservada switch y seguido de la variable o expresión a evaluar, pero sin ningún operador de comparación.

>switch (expresion) {}

Después colocamos cada caso con la palabra reservada case y el valor que deberá ser igual a la expresión. Seguido colocamos el bloque de código a ejecutar y al final la palabra reservada break para que no vuelva a evaluar otra condición si ya se cumplió.

>switch (expresion) { <br>
> case 1: { <br>
>        // Bloque 1 <br>
>        break <br>
> } <br>
> case 2: { <br>
>        // Bloque 2 <br>
>        break <br>
>    } <br>
>} <br>

Finalmente, colocamos la condición por defecto con la palabra reservada default que se ejecutará si ninguno de los casos fue el correcto. Esto es semejante al bloque else.

>switch (expresion) { <br>
>  case 1: { <br>
>    // Bloque 1 <br>
>    break <br>
>  } <br>
>  case 2: { <br>
>   // Bloque 2 <br>
>    break <br>
>  } <br>
>  default: { <br>
>    // Bloque por defecto <br>
>  } <br>
>} <br>

Esto se leería de la siguiente manera: evalúa (switch) la variable expresion, en el caso de que sea igual a uno (case 1), entonces ejecuta el bloque 1 y termina (break), en el caso de que sea igual a dos (case 2), entonces ejecuta el bloque 2 y termina (break), si no se cumple ninguna, ejecuta un bloque por defecto (default).

Ejemplo utilizando switch
Por ejemplo, creemos un semáforo.

>function semaforo(color) { <br>
>  switch (color) { <br>
>    case "verde": { <br>
>      console.log("¡Sigue!") <br>
>      break <br>
>    } <br>
>    case "amarillo": { <br>
>      console.log("¡Detente!") <br>
>      break <br>
>    } <br>
>    case "rojo": { <br>
>      console.log("¡No puedes avanzar!") <br>
>      break <br>
>    } <br>
>    default: { <br>
>      console.log("¡No reconozco ese color! :(") <br>
>    } <br>
>  } <br>
>} <br>
> <br>
>semaforo("verde") //'¡Sigue!' <br>

**Cuándo utilizar switch**

Deberías utilizar switch cuando tengas una gran cantidad de casos, que con el condicional if produciría más cantidad de código. El problema con switch es que no es muy utilizado y todo se resuelve con if. Sin embargo, conocer esta estructura te puede permitir escribir código más legible en ciertos casos.

-------------------------------
*Ejercicio de condicionales*

Cambia tu juego de piedra, papel o tijera realizado con condicionales if a la estructura switch. ¿Qué diferencias observaste? ¡Comparte tu trabajo en la sección de aportes!

-----------------------------------------------------------------
**Lecturas recomendadas**

[GitHub - degranda/jsBasico-: Ejemplos del curso de JS básico](https://github.com/degranda/jsBasico)
