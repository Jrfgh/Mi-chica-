<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>¡Diviértete con Tu Amor!</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
        }
        h1 {
            color: #FF69B4;
        }
        p {
            color: #333;
        }
        #diversion {
            margin-top: 50px;
        }
    </style>
    <script>
        function mostrarRespuesta() {
            var respuesta = document.getElementById("respuesta");
            respuesta.innerHTML = "¡Estamos en las mismas hojas!";
        }
    </script>
</head>
<body>
    <h1>¡Bienvenida a la diversión con tu amor!</h1>
    <div id="diversion">
        <p>Aquí tienes algo especial para hacer sonreír tu día:</p>
        <p>1. <a href="#" onclick="mostrarRespuesta()">¿Qué le dice un jardinero a otro?</a> <br> 2. <a href="https://www.minijuegos.com/juego/2048">¡Juega al emocionante juego 2048!</a> <br> 3. <a href="https://emojipedia.org/es/coraz%C3%B3n-azul-claro">¡Echa un vistazo a este hermoso corazón azul claro!</a></p>
        <p id="respuesta"></p>
    </div>
</body>
</html>
