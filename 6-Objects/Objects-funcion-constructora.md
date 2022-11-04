***Objects: Función constructora***

Existe un problema al momento de construir varios objetos a partir de un código base, los atributos deben cambiar con respecto a la nueva información. Para esto se utiliza una función constructora.

Una función constructora sirve para crear varios objetos a partir de nueva información, esto es recibido argumentos.

**Cómo generar varios objetos a partir de una función constructora**

Para crear una función constructora, debemos definir los parámetros correspondientes, que serán los atributos del objeto, que cambiarán con la nueva información mediante argumentos. Estos argumentos deben hacer referencia a cada uno del nuevo objeto, esto mediante el objeto contexto this.

Ten en cuenta que los parámetros de la función son diferentes a los atributos del objeto 😄.

``function Auto(brand, model, year){`` <br>
``    this.marca = brand`` <br>
``    this.modelo = model`` <br>
``    this.año = year`` <br>
``    this.detalle = function () {`` <br>
``        console.log(`Auto ${this.modelo} del ${this.año}.`)`` <br>
``    }`` <br>
``}`` <br>

Si ejecutamos la función Auto mostrará un error, necesitamos especificar que vamos a construir una instancia mediante la palabra reservada new.

``var miAuto = new Auto("Toyota", "Corolla", 2020)`` <br>
``/*Auto {`` <br>
``  marca: 'Toyota',`` <br>
``  modelo: 'Corolla',`` <br>
``  'año': 2020,`` <br>
``  detalle: ƒ ()`` <br>
``}*/`` <br>

De esta manera, puedes crear varios objetos a partir de una función constructora que permita especificar atributos y métodos personalizados.

``var otroAuto = new Auto("Tesla", "Model 3", 2021)`` <br>
``var otroAuto2 = new Auto("Suzuki", "K-20", 2019)`` <br>
``var otroAuto3 = new Auto("Ferrari", "Model N", 2018)`` <br>

Puede que observes la propiedad ``__proto__``, no te preocupes, ya lo aprenderás.

***Próximos pasos***
El tema de objetos es extenso, por lo que te dejaré los respectivos cursos del tema:

- [Curso de Programación Orientada a Objetos: POO](https://platzi.com/cursos/oop/)
- [Curso Básico de Programación Orientada a Objetos con JavaScript](https://platzi.com/cursos/javascript-poo/)
- [Curso Intermedio de Programación Orientada a Objetos en JavaScript](https://platzi.com/cursos/javascript-poo-intermedio/)

----------------------------------------------------------------

Lecturas recomendadas

[GitHub - degranda/jsBasico-: Ejemplos del curso de JS básico](https://github.com/degranda/jsBasico)
