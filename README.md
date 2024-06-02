<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Clicker Game</title>
<style>
    body {
        display: flex;
        justify-content: center;
        align-items: center;
        height: 100vh;
        margin: 0;
        font-family: Arial, sans-serif;
    }
    .clicker-container {
        text-align: center;
    }
    .clicker-button {
        padding: 20px 40px;
        font-size: 24px;
        cursor: pointer;
        background-color: #007bff;
        color: white;
        border: none;
        border-radius: 10px;
        outline: none;
    }
    .counter {
        font-size: 36px;
        margin-top: 20px;
    }
</style>
</head>
<body>
    <div class="clicker-container">
        <button class="clicker-button" onclick="incrementCounter()">Click Me!</button>
        <div class="counter">Count: <span id="count">0</span></div>
    </div>

    <script>
        let count = 0;

        function incrementCounter() {
            count++;
            document.getElementById('count').textContent = count;
        }
    </script>
</body>
</html>
