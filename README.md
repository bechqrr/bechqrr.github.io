<!DOCTYPE html>
<html>
<head>
    <title>Site de Bechirr</title>
    <style>
        body {
            background: linear-gradient(145deg, #290537, #310541);
            box-shadow: 33px 33px 66px #270434, -33px -33px 66px #350646;
            color: gold;
            font-family: Arial, sans-serif;
        }
        
        h1 {
            font-style: italic;
        }

        .btn {
            font-size: 24px;
            background: none;
            border: none;
            cursor: pointer;
            position: relative;
        }

        .btn strong {
            display: block;
            margin-bottom: 10px;
        }

        #container-stars {
            position: absolute;
            width: 100%;
            height: 100%;
            top: 0;
            left: 0;
            overflow: hidden;
        }

        #stars {
            position: absolute;
            width: 100%;
            height: 100%;
            background: url(stars.png) repeat top center;
            animation: animateStars 5s linear infinite;
        }

        @keyframes animateStars {
            0% {
                transform: translateY(0);
            }
            100% {
                transform: translateY(-100%);
            }
        }

        #glow {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            width: 80px;
            height: 80px;
            animation: glow 2s ease-in-out infinite;
        }

        .circle {
            position: absolute;
            width: 80px;
            height: 80px;
            border-radius: 50%;
            background: radial-gradient(#fff, transparent);
            animation: pulse 2s ease-in-out infinite;
        }

        @keyframes glow {
            0% {
                box-shadow: 0 0 5px gold;
            }
            50% {
                box-shadow: 0 0 20px gold, 0 0 40px gold, 0 0 60px gold, 0 0 80px gold;
            }
            100% {
                box-shadow: 0 0 5px gold;
            }
        }

        @keyframes pulse {
            0% {
                transform: scale(0);
            }
            50% {
                transform: scale(1);
                opacity: 1;
            }
            100% {
                transform: scale(0);
            }
        }
    </style>
</head>
<body>
    <button class="btn" type="button">
        <strong>bechirr</strong>
        <div id="container-stars">
            <div id="stars"></div>
        </div>

        <div id="glow">
            <div class="circle"></div>
            <div class="circle"></div>
        </div>
    </button>
    <h1>Bechirr</h1>
    <p><strong>Snapchat:</strong> <a href="https://www.snapchat.com/add/bechir_du26" target="_blank">bechir_du26</a></p>
    <p><strong>Instagram:</strong> <a href="https://www.instagram.com/bechiqr26" target="_blank">bechiqr26</a></p>
    <p><strong>TikTok:</strong> <a href="https://www.tiktok.com/@bechirr" target="_blank">.bechirr</a></p>
</body>
</html>
