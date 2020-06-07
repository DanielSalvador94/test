<h1>Test-2</h1>
El fragmento de código de nuestro fichero test.js nos devuelve un output no deseado. Queremos imprimir un valor incremental a cada segundo pero lo que nos devuelve el código es el mismo valor en cada iteración.

Sin necesidad de ejecutar el código, ¿sabrías decirnos qué valor imprimiría por consola el script? ¿Cuál es el motivo?
Sabiendo que el output que buscamos es el que encuentras bajo estas líneas… ¿Cómo solucionarías el fragmento de código para que el output sea el deseado?
<ul>
<li>>0</li>
<li>>1</li>
<li>>2</li>
<li>>3</li>
<li>>4</li>
</ul>
<h2>Solucion</h2>
<ul>
<li>Imprimiría cinco veces el numero 5,Es debido a que dentro del bucle for se declara el indice con var a nivel global</li>
<li>Una solución seria sustituir la declaracion del indice "var" por "let" de esta manera for (let i = 0; i < 5; i++) limitando asi el alcance de la variable a dentro del bucle y cambiando su valor en cada iteracion</li>
</li>
</ul>
