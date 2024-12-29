Fortune
<!DOCTYPE html>
<html lang="pt">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Jogo de Roleta</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #282c34;
            color: white;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }
        #roleta {
            width: 300px;
            height: 300px;
            background-color: #f00;
            border-radius: 50%;
            margin: 20px;
            transition: transform 4s ease-out;
        }
        button {
            padding: 10px 20px;
            font-size: 16px;
            color: white;
            background-color: #4CAF50;
            border: none;
            cursor: pointer;
            border-radius: 5px;
        }
        button:hover {
            background-color: #45a049;
        }
    </style>
</head>
<body>

    <h1>Jogo de Roleta</h1>
    <div id="roleta"></div>
    <button onclick="rodarRoleta()">Rodar</button>

    <script>
        function rodarRoleta() {
            const roleta = document.getElementById("roleta");
            const graus = Math.floor(Math.random() * 360);
            roleta.style.transform = `rotate(${graus}deg)`;
        }
    </script>

</body>
</html>
