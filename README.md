<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Сюрприз</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: white;
            margin: 0;
            font-family: Arial, sans-serif;
            flex-direction: column;
        }
        .heart {
            font-size: 100px;
            color: red;
            animation: beat 1s infinite;
        }
        @keyframes beat {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.2); }
        }
        .text {
            font-size: 24px;
            margin-top: 20px;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <div class="heart">♥️</div>
    <div class="text" onclick="showLove()">нажми</div>

    <script>
        function showLove() {
            document.querySelector('.text').innerText = 'люблю тебя';
        }
    </script>
</body>
</html>
