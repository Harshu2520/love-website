# love-website
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>For My Love</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #ffebf0;
            text-align: center;
            padding: 50px;
        }
        .container {
            background: white;
            padding: 20px;
            border-radius: 15px;
            box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.1);
            display: inline-block;
        }
        h1 {
            color: #ff4d6d;
        }
        .heart {
            color: red;
            font-size: 50px;
            animation: heartbeat 1s infinite;
        }
        @keyframes heartbeat {
            0% { transform: scale(1); }
            50% { transform: scale(1.2); }
            100% { transform: scale(1); }
        }
        button {
            background: #ff4d6d;
            color: white;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            margin-top: 10px;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>For My Love ❤️</h1>
        <p id="loveMessage">You are the most beautiful person in my life!</p>
        <div class="heart">❤️</div>
        <button onclick="showLoveMessage()">Show Love Quote</button>
    </div>

    <script>
        const loveQuotes = [
            "You are my sunshine on a cloudy day! ☀️",
            "I love you more than words can express! 💖",
            "Every moment with you is a treasure! 🥰",
            "You make my world brighter! ✨",
            "I am so lucky to have you in my life! 💞"
        ];

        function showLoveMessage() {
            const randomIndex = Math.floor(Math.random() * loveQuotes.length);
            document.getElementById("loveMessage").innerText = loveQuotes[randomIndex];
        }
    </script>
</body>
</html>
