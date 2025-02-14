<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Be My Valentine?</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background: linear-gradient(to bottom, #87CEEB, #FFFFFF);
            margin: 0;
            padding: 50px;
        }
        h1 {
            color: #ff4d4d;
        }
        .container {
            margin-top: 50px;
        }
        .btn {
            font-size: 20px;
            padding: 10px 20px;
            margin: 10px;
            border: none;
            border-radius: 10px;
            cursor: pointer;
            transition: 0.3s;
        }
        .yes {
            background-color: #ff4d4d;
            color: white;
        }
        .no {
            background-color: #cccccc;
            color: black;
            position: absolute;
        }
    </style>
</head>
<body>
    <h1>Will you be my Valentine, Farhanaaa? 💖</h1>
    <div class="container">
        <button class="btn yes" onclick="showLoveMessage()">Yes</button>
        <button class="btn no" id="noButton" onmouseover="moveButton()">No</button>
    </div>

    <script>
        function moveButton() {
            var x = Math.random() * (window.innerWidth - 100);
            var y = Math.random() * (window.innerHeight - 50);
            document.getElementById('noButton').style.left = x + 'px';
            document.getElementById('noButton').style.top = y + 'px';
        }

        function showLoveMessage() {
            setInterval(function() {
                alert('Yay! I love you bby ❤️');
            }, 500);
        }
    </script>
</body>
</html>
