<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ÆTHER</title>
    <style>
        /* Reset and base styles */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            -webkit-font-smoothing: antialiased;
        }

        :root {
            --primary: #0a0a0a;
            --accent: #ff375f;
            --spacing: 2rem;
        }

        body {
            background: #ffffff;
            font-family: 'Neue Machina', system-ui, sans-serif;
            color: var(--primary);
            line-height: 1.2;
            overflow-x: hidden;
        }

        /* Layout structure */
        .frame {
            min-height: 100vh;
            display: grid;
            grid-template-rows: auto 1fr auto;
            padding: var(--spacing);
        }

        /* Logo treatment */
        .logo-container {
            position: relative;
            margin: 10vh auto;
            max-width: 1200px;
            isolation: isolate;
        }

        .logo-container img {
            width: 100%;
            height: auto;
            filter: contrast(120%);
            border: 1px solid var(--primary);
            box-shadow: 16px 16px 0 var(--accent);
            transition: transform 0.6s cubic-bezier(0.16, 1, 0.3, 1);
        }

        .logo-container:hover img {
            transform: translate(-8px, -8px);
            box-shadow: 24px 24px 0 var(--accent);
        }

        /* Contact section */
        .contact {
            text-align: center;
            padding: calc(var(--spacing) * 2) 0;
            position: relative;
        }

        .contact::before {
            content: '';
            position: absolute;
            top: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 120px;
            height: 3px;
            background: var(--primary);
        }

        .contact a {
            color: var(--primary);
            text-decoration: none;
            font-size: 1.5rem;
            letter-spacing: -0.03em;
            position: relative;
            padding: 0.75rem 2rem;
            display: inline-block;
        }

        .contact a::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 100%;
            height: 2px;
            background: var(--accent);
            transform: scaleX(0);
            transition: transform 0.4s ease-out;
        }

        .contact a:hover::after {
            transform: scaleX(1);
        }

        /* Responsive adjustments */
        @media (max-width: 768px) {
            :root {
                --spacing: 1rem;
            }

            .logo-container img {
                box-shadow: 8px 8px 0 var(--accent);
            }

            .logo-container:hover img {
                transform: translate(-4px, -4px);
                box-shadow: 12px 12px 0 var(--accent);
            }
        }

    </style>
    <link href="https://fonts.cdnfonts.com/css/neue-machina" rel="stylesheet">
</head>
<body>
    <div class="frame">
        <main class="logo-container">
            <img src="https://i.ibb.co/xtJk2gk7/text-1739414566378.png" alt="ÆTHER agency logo">
        </main>

        <footer class="contact">
            <a href="mailto:booking@aetherlive.net">BOOKING@AETHERLIVE.NET</a>
        </footer>
    </div>
</body>
</html>
