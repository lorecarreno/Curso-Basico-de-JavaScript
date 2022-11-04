**Eliminando elementos de un Array**

El método *.push()* nos permite agregar uno o más elementos al final de un array. A continuación veremos un ejemplo aplicado con un array que contiene números:

``// Array inicial`` <br>
``let numArray = [1, 2, 3, 4, 5]`` <br>
`` `` <br>
``// Función`` <br>
``function newNum (){`` <br>
``    // Agrego elementos`` <br>
``    numArray.push(6, 7)`` <br>
``    // Reviso el array que ahora tiene los numeros agregados``
``    console.log(numArray)`` <br>
``}`` <br>

>undefined

`` // Ejecuto la función`` <br>
`` newNum()`` <br>

> (7) [1,2,3,4,5,6,7]

Como podemos ver, al momento de ejecutar la función se agregan los números 6 y 7 al array. Ahora revisemos un ejemplo con strings:

``// -- Ejemplo con strings`` <br>
``// Array inicial`` <br>
``let txtArray = ["Lore", "Milo", "Nano", "Mawsi"]`` <br>
`` `` <br>
``// Función`` <br>
``function addCharacters (){`` <br>
``    // Agrego elementos`` <br>
``    txtArray.push("Benito","Fusi")`` <br>
``    // Reviso el array que ahora tiene los numeros agregados`` <br>
``    console.log(txtArray)`` <br>
``}`` <br>

>undefined

``addCharacters()`` <br>

> (6) ["Lore", "Milo", "Nano", "Mawsi","Benito","Fusi"]

Como podemos ver, agregamos dos cadenas de strings al ejecutar la función donde tenemos *txtArray.push()*. Es decir, indico el array al que voy agregar elementos, uso el método *.push()*, y dentro de *.push()* indico los elementos que quiero agregar al string. Finalmente, el console.log() lo uso para revisar en la consola si esto sucedió o no.

**.shift()**

Ahora pasemos a la otra cara de la moneda donde necesitamos eliminar un elemento del array. .shift() eliminar el primer elemento de un array, es decir, elimina el elemento que esté en el índice 0.

`` //Creamos un array`` <br>
``let array = [1, 2, 3, 4, 5]`` <br>
`` console.log(array)`` <br>
`` `` <br>
`` //Aplicamos .shift()`` <br>
``let shiftArray = array.shift()`` <br>
`` `` <br>
`` //Revisamos. El output debe ser [2,3,4,5]`` <br>
`` console.log(array)`` <br>

>(5) [1, 2, 3, 4, 5]
>(4) [2, 3, 4, 5]

Como vemos, luego de aplicar *.shift()* se eliminó exitosamente el primer elemento del array. ¿Y si quisiéramos eliminar el último elemento? Pasemos al bonus track de esta clase 🙌🏼.

**Bonus Track**

Si ya entendiste cómo funciona *.shift()* aplicar *.pop()* te será pan comido 🍞. El método *.pop()* eliminará el último elemento de un array. En este sentido, si tenemos un array de 5 elementos, pop() eliminará el elemento en el índice 4. Utilicemos el mismo ejemplo pero usando este método.

``let array = [1, 2, 3, 4, 5]`` <br>
``console.log(array)`` <br>
`` `` <br>
``//Aplicamos .pop()`` <br>
``let shiftArray = array.pop()`` <br>
`` `` <br>
``//Revisamos. El output debe ser [1, 2, 3, 4]`` <br>
``console.log(array)`` <br>

¡Y listo! Ahora que ya conoces todos estos métodos te recomiendo comenzar a experimentar 💪🏼

👉🏾 Link al repositorio de esta clase: [https://github.com/aaronpaulgz/push-shift](https://github.com/aaronpaulgz/push-shift)
