<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ÆTHER</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background: #fff;
            font-family: 'Archivo Black', sans-serif;
            color: #111;
            min-height: 100vh;
            display: grid;
            grid-template-rows: 1fr auto;
        }

        .container {
            display: grid;
            place-items: center;
            padding: 2rem;
        }

        img {
            max-width: min(90vw, 800px);
            height: auto;
            border: 4px solid #111;
            box-shadow: 12px 12px 0px #e63946;
            transition: transform 0.3s ease;
        }

        img:hover {
            transform: rotate(-0.5deg);
        }

        .contact {
            text-align: center;
            padding: 3rem;
            border-top: 4px solid #111;
            background: #f8f9fa;
        }

        a {
            color: #e63946;
            text-decoration: none;
            font-size: 1.5rem;
            position: relative;
            padding: 0.5rem 1rem;
            display: inline-block;
        }

        a::before {
            content: '';
            position: absolute;
            width: 100%;
            height: 100%;
            border: 2px solid #111;
            top: 4px;
            left: 4px;
            transition: all 0.3s ease;
        }

        a:hover::before {
            top: 0;
            left: 0;
        }

        @media (max-width: 768px) {
            img {
                box-shadow: 6px 6px 0px #e63946;
            }
            
            a {
                font-size: 1.2rem;
            }
        }
    </style>
    <link href="https://fonts.googleapis.com/css2?family=Archivo+Black&family=Space+Mono:wght@400;700&display=swap" rel="stylesheet">
</head>
<body>
    <div class="container">
        <img src="https://i.ibb.co/xtJk2gk7/text-1739414566378.png" alt="ÆTHER">
    </div>

    <div class="contact">
        <a href="mailto:booking@aetherlive.net">BOOKING@AETHERLIVE.NET</a>
    </div>
</body>
</html>
