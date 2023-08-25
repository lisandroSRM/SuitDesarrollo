# hola mundo 

-Para hacer una pagina web con php primero debemos de activar el puerto con xampp
![[Pasted image 20230824073619.png]]
-Crear una carpeta  con vs dentro de htdocs creamos un archivo index donde comenzaremos la estructura de html
-Abrimos la carpeta y comenzamos a crear nuestros archivos con extensión .php .html .css etc.
-Para poder utilizar código PHP demos de escribir dentro de un bloque PHP y este se declara así <?php?>

### Variables 
Para declarar variables en código PHP se declararan con $, aparte de que PHP es un lenguaje interpretado.
````
<?php

$nombre ="lisandro";

$edad = 21;

$mayor_edad = true;

var_dump($nombre);

var_dump($edad);

var_dump($mayor_edad);

  

//definicion de constantes

  

define("pi", 3.1314);// de esta manera se declara una constatnte en php

  

print ("Mi nombre es". $nombre); //La concatenacion se hace con punto

  
  

?>
````
### Constantes 
Las variables en PHP se definen con define() y esta debe de llevar nombre y puede llevar cualquier tipo de dato.
### Operaciones Aritméticas

````
<?php

print(5+4);//suma

echo"<br>";

print(5-4);//resta

echo"<br>";

print(5*4);//mult

echo"<br>";

print(5/4);

echo"<br>";//div

print(10%2);

echo"<br>";//modulo

print(2**2);//potencia

?>

````
### Operaciones Lógicas
| nombre | simbolo |
|---|----------|
|AND|AND &&|
|OR|OR | |
|NOT|!|
````
<?php

//tabla de verdad de AND

var_dump(false && false);

var_dump(false && true);

var_dump(true && false);

var_dump(true && true);

  

//tabla de verdad de OR

var_dump(false | false);

var_dump(false | true);

var_dump(true | false);

var_dump(true | true);

  

?>
````
### Else if
Es una pregunta en programación que evalúa una respuesta o varias dependiendo la situación.
````
<?php

$edad =40;

if($edad >=18 and $edad <30){

    print("eres mayor de edad");

}else if($edad >=30){

    print("eres adulto");

}else if($edad >= 60){

    print("eres adulto mayor");

}else

print("eres menor de edad");

?>
````
### Switch
Estructura de control que nos permite poner una cantidad de opciones para una respuesta y tambien colocar un default en caso de no contar con la opcion para la respuesta.
````
<?php

$opcion ="HTML";

switch($opcion){

    case  'HTML':

        print("Lenguaje de maquetado");

        break;

    case  'CSS':

        print("hoja de estilo");

        break;

    case  'JS':

        print("lenguaje de programacion cliente");

        break;

    default:

        print("no conozco ese lenguaje");

        break;

}
?>
````
### While y Do While
Es un bucle que se ejecutara hasta el LIMITE  que nosotros pongamos, primero evalúa y luego ejecuta. 
````
<?php

$a=0;

  

while($a <=10){

    print($a);

    $a++;

}

  

do{

    print($a);

    $a++;

}while ($a <=10);

  
  

?>
````
### Arreglos
Estos son un conjunto de elementos también podrían ser llamados listas, existen de un solo tipo de dato o puedes hacerlo mixto.
````
<?php

$calificaciones = [100,99,89,78,67,78];

$arreglo =["hola mundo", 24, true];

  

echo "<pre>";

print_r($calificaciones);

echo "</pre>" //da formato agregando saltoa de linea al arreglo

  

?>
````
### Arreglos Asociativos
Se toma de un arreglo informacion mediante las llaves y dentro de estas llaves existe más informacion y podemos llegar a esta especificando las llaves.
````
<?php

    $persona = [

  

        "nombre" => "Lisandro",

        "edad" => 21,

        "direccion" => [

            "cuidad" => "CDMX",

            "Alcaldia" => "Milpa Alta",

            "Pueblo" => "Santa Ana Tlacotenco"

        ],

         "calificaciones" => [12,23,45,65,78,99]

        ];

    echo "<pre>";

  

    print_r ($persona);

  

    print ($persona["direccion"]["Alcaldia"]);

  

    print ($persona["calificaciones"][3]);

  

    echo "</pre>";

  

?>
````
### For
Es un bucle que puede recorrer arreglos y mostrarnos los valores del mismo y se terminara en el LIMITE que nosotros le indiquemos.

````
<?php

    $calificaciones = [100,90,80,78,67,78];

    $arreglo = ["hola", 23, true];

    for($i = 0; $i < count($calificaciones); $i++){

        print ($calificaciones[$i]);

        echo "<br>";

    }

    echo "<br>";

    for($i = 0; $i < count($arreglo); $i++){

        print ($arreglo[$i]);

        echo "<br>";

    }

?>
````
