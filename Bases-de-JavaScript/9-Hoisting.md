***Hoisting***


*Hoisting* es un término para describir que las declaraciones de variables y funciones son desplazadas a la parte superior del scope más cercano, scope global o de función. Esto sucede solamente con las declaraciones y no con las asignaciones.

El código permanece igual, solo es una interpretación del motor de JavaScript. En el caso de las variables solamente sucede cuando son declaradas con var.

**Hoisting en variables declaradas con var**

Mira el siguiente código, ¿qué crees que sea el resultado del console.log?

>console.log(nombre) // undefined <br>
>var nombre = "Andres" <br>

La respuesta del console.log es undefined, porque al hacer referencia a una variable que no está declarada aún, JavaScript crea esta variable antes de declararla y le asigna un valor de undefined.

Lo que JavaScript está haciendo sería lo siguiente:

>// Hoistin: Declara y asigna undefined <br>
>var nombre = undefined <br>
>console.log(nombre) // undefined <br>
>nombre = "Andres" <br>

Aquí el nombre de Hoisting o elevación.

**Hoisting en funciones**

Mira el siguiente código, ¿qué crees que sea el resultado del console.log?

>console.log( saludar() ) <br>
> <br>
>function saludar() { <br>
> return "Hola" <br>
>} <br>

La respuesta es "Hola", porque al invocar una función que no está declarada, JavaScript la eleva y por eso podemos invocar una función antes de declararla.

>// Hoisting: Declara la función antes de ser invocada <br>
>function saludar() { <br>
> return "Hola" <br>
>} <br>
> <br>
>console.log( saludar() ) // "Hola" <br>

Pero, lo que realmente sucede es que JavaScript guarda la función en memoria en la fase de creación de un contexto de ejecución, no asigna undefined como con las variables.

**Buenas prácticas**

El tema de Hoisting solo sucede con las declaraciones de variables y funciones, por lo que _se recomienda declarar las variables y las funciones lo más arriba posible del código_, para evitar errores.

También, el tema de hoisting ya está solucionado con las [nuevas formas de declarar variables](https://platzi.com/clases/3504-ecmascript-nuevo/51753-let-y-const-y-arrow-functions/) con let y const.

----------------------------------------------------------------
**Lecturas recomendadas**

[Curso de ECMAScript 6+](<https://platzi.com/clases/ecmascript-6/>)

[Hoisting - Glosario | MDN](https://developer.mozilla.org/es/docs/Glossary/Hoisting)

[¿Qué es el hoisting? - Ana Martínez Aguilar - Medium](https://medium.com/@anamartinezaguilar/qu%C3%A9-es-el-hoisting-327870f67b36)

[GitHub - degranda/jsBasico-: Ejemplos del curso de JS básico](https://github.com/degranda/jsBasico)


