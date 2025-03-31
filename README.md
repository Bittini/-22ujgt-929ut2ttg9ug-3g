<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Random Number Generator</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            padding: 50px;
        }
        #number {
            font-size: 2em;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <h1>Infinite Random Number Generator</h1>
    <div id="number">77,579.62</div>

    <script>
        function generateRandomNumber() {
            let randomNum = (Math.random() * 100000).toFixed(2);
            document.getElementById("number").textContent = randomNum;
        }
        
        setInterval(generateRandomNumber, 500); // Generate a new number every 500ms
    </script>
</body>
</html>
