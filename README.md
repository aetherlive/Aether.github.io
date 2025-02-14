<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ÆTHER | Electronic Music Production</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background: #000;
            font-family: 'Space Mono', monospace;
            color: #0ff;
            overflow-x: hidden;
        }

        .container {
            height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            position: relative;
        }

        img {
            max-width: 80vw;
            height: auto;
            filter: grayscale(100%) contrast(130%);
            transition: filter 0.8s;
            border: 3px solid #f0f;
        }

        img:hover {
            filter: grayscale(0%) contrast(100%);
        }

        .contact {
            position: fixed;
            bottom: 2rem;
            left: 50%;
            transform: translateX(-50%);
            font-size: 1.2rem;
            text-align: center;
            mix-blend-mode: difference;
        }

        a {
            color: #f0f;
            text-decoration: none;
            position: relative;
        }

        a::after {
            content: '';
            position: absolute;
            bottom: -2px;
            left: 0;
            width: 0;
            height: 2px;
            background: #0ff;
            transition: width 0.3s;
        }

        a:hover::after {
            width: 100%;
        }

        .scanline {
            position: fixed;
            width: 100%;
            height: 2px;
            background: #0ff;
            animation: scan 4s linear infinite;
        }

        @keyframes scan {
            0% { top: -2px; }
            100% { top: 100%; }
        }

    </style>
    <link href="https://fonts.googleapis.com/css2?family=Space+Mono:wght@400;700&family=Inconsolata:wght@900&display=swap" rel="stylesheet">
</head>
<body>
    <div class="scanline"></div>
    
    <div class="container">
        <img src="https://i.ibb.co/xtJk2gk7/text-1739414566378.png" alt="ÆTHER">
    </div>

    <div class="contact">
        <a href="mailto:booking@aetherlive.net">BOOKING@AETHERLIVE.NET</a>
    </div>

</body>
</html>
