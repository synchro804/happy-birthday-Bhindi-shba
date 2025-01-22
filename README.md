<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Birthday, Noor Zainab!</title>
    
    <!-- Import Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@700&display=swap" rel="stylesheet">
    
    <style>
        body {
            font-family: 'Dancing Script', cursive;
            background-color: black;
            color: gold;
            text-align: center;
            padding: 50px;
            margin: 0;
            position: relative;
            overflow: hidden;
        }

        .message-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }

        .word {
            font-size: 3em;
            margin: 10px;
            opacity: 0;
            transform: translateY(50px);
            animation: slideIn 0.8s ease-out forwards;
        }

        .birthday-message {
            font-size: 4em;
            font-weight: bold;
            color: #FFD700;
            animation: fadeIn 2s ease-in-out;
        }

        @keyframes slideIn {
            0% {
                opacity: 0;
                transform: translateY(50px);
            }
            100% {
                opacity: 1;
                transform: translateY(0);
            }
        }

        @keyframes fadeIn {
            0% {
                opacity: 0;
            }
            100% {
                opacity: 1;
            }
        }

        .highlight {
            color: #FFD700;
            font-size: 1.5em;
        }

        p {
            font-size: 1.2em;
            margin: 20px;
        }

        /* 3D Balloon Styles */
        .balloon {
            position: absolute;
            bottom: -100px;
            width: 50px;
            height: 80px;
            background-color: #FFD700;
            border-radius: 50%;
            animation: float 8s ease-in-out infinite, sway 2s ease-in-out infinite;
        }

        .balloon:nth-child(2) {
            background-color: #ff5733;
            animation-delay: 1s;
        }

        .balloon:nth-child(3) {
            background-color: #33ff57;
            animation-delay: 2s;
        }

        .balloon:nth-child(4) {
            background-color: #ff33a1;
            animation-delay: 3s;
        }

        /* Balloon floating and swaying animation */
        @keyframes float {
            0% {
                bottom: -100px;
                transform: scale(1) rotate(0deg);
            }
            100% {
                bottom: 100vh;
                transform: scale(1.2) rotate(360deg);
            }
        }

        @keyframes sway {
            0% {
                transform: rotate(0deg);
            }
            50% {
                transform: rotate(10deg);
            }
            100% {
                transform: rotate(-10deg);
            }
        }

        /* Fireworks effect */
        .fireworks {
            position: absolute;
            top: 50%;
            left: 50%;
            width: 0;
            height: 0;
            border-radius: 50%;
            background-color: rgba(255, 223, 0, 0.8);
            animation: fireworks-animation 2s linear infinite;
        }

        @keyframes fireworks-animation {
            0% {
                width: 5px;
                height: 5px;
                opacity: 0.9;
            }
            25% {
                width: 30px;
                height: 30px;
                opacity: 1;
            }
            50% {
                width: 50px;
                height: 50px;
                opacity: 0.7;
            }
            100% {
                width: 100px;
                height: 100px;
                opacity: 0;
                transform: scale(1.2);
            }
        }

    </style>
</head>
<body>

    <div class="message-container">
        <!-- Birthday Message with Animation -->
        <div class="birthday-message">
            <span class="word" style="animation-delay: 0.1s;">🎉</span>
            <span class="word" style="animation-delay: 0.2s;">🎂</span>
            <span class="word" style="animation-delay: 0.3s;">Happy</span>
            <span class="word" style="animation-delay: 0.4s;">Birthday,</span>
            <span class="word" style="animation-delay: 0.5s;">Noor</span>
            <span class="word" style="animation-delay: 0.6s;">Zainab!</span>
            <span class="word" style="animation-delay: 0.7s;">🎈</span>
            <span class="word" style="animation-delay: 0.8s;">🎉</span>
        </div>
    </div>

    <p class="highlight">Noor Zainab, you are a shining star in the lives of everyone around you. </p>
    <p>Your kindness, warmth, and genuine spirit make the world a better place. You possess a heart of gold and a beauty that radiates both inside and out. May your day be filled with as much love and happiness as you give to others every day!</p>
    <p>Enjoy your special day, Noor! 🎉💖</p>

    <!-- 3D Balloons -->
    <div class="balloon" style="left: 10%;"></div>
    <div class="balloon" style="left: 30%;"></div>
    <div class="balloon" style="left: 50%;"></div>
    <div class="balloon" style="left: 70%;"></div>

    <!-- Fireworks -->
    <div class="fireworks" style="top: 20%; left: 30%;"></div>
    <div class="fireworks" style="top: 40%; left: 60%;"></div>
    <div class="fireworks" style="top: 60%; left: 80%;"></div>

    <script>
        // Function to add word-by-word animation delay dynamically
        document.addEventListener('DOMContentLoaded', () => {
            const words = document.querySelectorAll('.word');
            words.forEach((word, index) => {
                word.style.animationDelay = `${index * 0.2}s`;
            });
        });
    </script>

</body>
</html>
