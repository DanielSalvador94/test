<h1>Test-1</h1>
Para responder a este test encontrarás un archivo llamado test.js en esta misma carpeta donde hay un pequeño fragmento de código que deberás analizar y responder a las siguientes cuestiones.

<ul>
<li>En el fragmento de código de nuestro archivo (script.js) podemos encontrar hasta 3 variables. ¿Podrías decirnos cuál sería el valor de todas ellas al finalizar la ejecución del script?</li>
  
<li>Modifica el código para que las variables rgb y wb mantengan sus valores iniciales y colors tenga los valores de ambas al finalizar la ejecución del script.</li>
<li>Además, tenemos un bug localizado en dispositivos con Internet Explorer… El código de nuestro script no funciona y necesitamos que se ejecute también en este navegador. ¿Sabrías identificar cuál es el problema? ¿Qué solución nos propones?</li>


PS: No es estrictamente necesario tener Internet Explorer para poder identificar y/o resolver el bug.

<h2>Solucion</h2>
1º EJERCICIO
-----------------------------------------------------------------------------------------------------------
1º VARIABLE { red: "#FF0000", green: "#00FF00", blue: "#0000FF", white: "#FFFFFF", black: "#000000" } -> Es decir tendra mergeados los colores de Rgb y de wb.
2º VARIABLE { white: "#FFFFFF", black: "#000000" } -> Es decir mantendrá los valores iniciales.
3º VARIABLE { red: "#FF0000", green: "#00FF00", blue: "#0000FF", white: "#FFFFFF", black: "#000000" } -> Es decir tendrá la combinación de Rgb y Wb.
---------------------------------------------------------------------------------------------------------
2º EJERCICIO
var colors ={
};
 Object.assign(colors,rgb,wb);
----------------------------------------------------------------------------------------------------------
3º EJERCICiO
-La funcion Assign no es compatible con internet Explorer, asi que se usará la funcion extend de Jquery que es compatible con el mismo.
-var rgb = {
    red: "#FF0000",
    green: "#00FF00",
    blue: "#0000FF"
};

var wb = {
    white: "#FFFFFF",
    black: "#000000"
};

var colors = $.extend( rgb, wb );
