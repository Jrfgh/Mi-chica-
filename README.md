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
        .calculator {
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        .calculator input {
            margin: 5px;
            padding: 10px;
            width: 200px;
            font-size: 18px;
        }
    </style>
</head>
<body>
    <h1>¡Bienvenida a la diversión junto a tu amor!</h1>
    <div id="diversion">
        <p>¡Aquí tienes algo especial para hacer sonreír tu día!</p>
        <ul>
            <li>¡Descubre un chiste encantador del día!</li>
            <li>¡Sumérgete en un juego sorpresa lleno de diversión!</li>
            <li>¡Deleita tus ojos con una galería de imágenes llenas de amor!</li>
        </ul>
        <p>¡Espero que te haga feliz!</p>
        <div class="calculator">
            <input type="text" id="input" readonly>
            <button onclick="clearInput()">C</button>
            <button onclick="appendToInput('7')">7</button>
            <button onclick="appendToInput('8')">8</button>
            <button onclick="appendToInput('9')">9</button>
            <button onclick="appendToInput('+')">+</button>
            <br>
            <button onclick="appendToInput('4')">4</button>
            <button onclick="appendToInput('5')">5</button>
            <button onclick="appendToInput('6')">6</button>
            <button onclick="appendToInput('-')">-</button>
            <br>
            <button onclick="appendToInput('1')">1</button>
            <button onclick="appendToInput('2')">2</button>
            <button onclick="appendToInput('3')">3</button>
            <button onclick="appendToInput('*')">*</button>
            <br>
            <button onclick="appendToInput('0')">0</button>
            <button onclick="appendToInput('.')">.</button>
            <button onclick="calculate()">=</button>
            <button onclick="appendToInput('/')">/</button>
        </div>
    </div>

    <script>
        function appendToInput(value) {
            document.getElementById('input').value += value;
        }

        function clearInput() {
            document.getElementById('input').value = '';
        }

        function calculate() {
            try {
                document.getElementById('input').value = eval(document.getElementById('input').value);
            } catch(error) {
                document.getElementById('input').value = 'Error';
            }
        }
    </script>
</body>
</html>
