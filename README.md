<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cambiar color de fondo</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin-top: 20%;
            transition: background-color 0.5s;
        }
        button {
            padding: 15px 30px;
            font-size: 18px;
            background-color: #333;
            color: white;
            border: none;
            cursor: pointer;
            border-radius: 8px;
        }
        button:hover {
            background-color: #555;
        }
    </style>
</head>
<body>
    <h1>¡Cambia el color de fondo!</h1>
    <button onclick="cambiarColor()">Cambiar color</button>

    <script>
        function cambiarColor() {
            // Genera un color aleatorio en formato hexadecimal
            let color = "#" + Math.floor(Math.random()*16777215).toString(16);
            document.body.style.backgroundColor = color;
        }
    </script>
</body>
</html>



