<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Encuesta de Clase</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f0f8ff; /* Color de fondo celeste */
            color: #333;
            text-align: center;
            margin: 0;
            padding: 0;
        }
        .container {
            max-width: 600px;
            margin: 50px auto;
            padding: 20px;
            background-color: #fff;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
        h1 {
            color: #ff4500; /* Color inspirado en "Cars" */
        }
        .question {
            font-size: 1.5em;
            margin-bottom: 20px;
        }
        .button {
            display: inline-block;
            padding: 15px 30px;
            margin: 10px;
            font-size: 1.2em;
            color: #fff;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            text-decoration: none;
        }
        .button.pink {
            background-color: #ff69b4; /* Rosado */
        }
        .button.blue {
            background-color: #87ceeb; /* Celeste */
        }
        .button:hover {
            opacity: 0.8;
        }
        .cars-image {
            width: 100%;
            max-width: 500px;
            height: auto;
            border-radius: 10px;
        }
        .message {
            font-size: 1.2em;
            margin-top: 20px;
            color: #ff4500; /* Color de texto */
            display: none; /* Inicialmente oculto */
        }
    </style>
</head>
<body>
    <div class="container">
        <img src="https://www.example.com/cars-image.jpg" alt="Cars" class="cars-image">
        <h1>Encuesta de Clase</h1>
        <p class="question">¿Qué tanto te gusta la clase?</p>
        <a href="#" class="button pink" onclick="showMessage('Lo sabía')">¡Me encanta!</a>
        <a href="#" class="button blue" onclick="showMessage('Estaré trabajando para mejorar')">Está bien</a>
        <p id="responseMessage" class="message"></p>
    </div>

    <script>
        function showMessage(message) {
            document.getElementById('responseMessage').textContent = message;
            document.getElementById('responseMessage').style.display = 'block';
        }
    </script>
</body>
</html>

