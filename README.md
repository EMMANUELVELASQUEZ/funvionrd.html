# funcion.html

<!DOCTYPE html>  
 <html>  
 <body>  
<body background bgcolor="PINK">
 <h1>Sumar dos numeros</h1>  
 <p><h2>Por favor, introduce dos numeros:</h2></p>  
 <input id="num1"><br>  
 <input id="num2">  
 <button type="button" onclick="myFunction()">Sumar</button>  
 <p id="sumando"></p>  
 <script>  
 function myFunction() {  
   var x,y,suma,text;  
   x = document.getElementById("num1").value;  
   y = document.getElementById("num2").value;  
   if (isNaN(x) || isNaN(y)) {  
     text = "Es necesarios introducir dos números válidos";  
   } else {  
     //si no ponemos parseFloat concatenaría x con y  
     suma=parseFloat(x)+parseFloat(y);  
     text= suma;  
   }  
   document.getElementById("sumando").innerHTML = text;  
 }  
 </script>  
 </body>  
 </html>  
 
 <meta charset="utf-8">
  <title>Trazo de texto</title>
  <style type="text/css">
    h1
    {
      color: lighcyan;
      -webkit-text-stroke: 2px yellow; /* prefijo de proveedor */
      font-size: 500%; /* aumenta el tamaño de la fuente */
    }
  </style>
</head>
<body>

<!-- Fig. 5.1: sombradetexto.html -->
<!-- Sombra de texto en CSS3. -->
<html>
<head>
  <meta charset="utf-8">
  <title>suma</title>
  <style type="text/css">
    h1
    {
      text-shadow: -10px 10px 10px red; /* agrega sombra */
      font-size: 500%; /* aumenta el tamaño de la fuente */
    }
