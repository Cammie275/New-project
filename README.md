<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Efek Glitch Keren</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: black;
            color: white;
            font-family: 'Courier New', monospace;
            text-align: center;
            overflow: hidden;
        }
        
        h1 {
            font-size: 50px;
            font-weight: bold;
            position: relative;
            text-transform: uppercase;
            color: white;
            animation: glitch 0.8s infinite;
        }

        @keyframes glitch {
            0% { transform: translate(0); }
            20% { transform: translate(-3px, 3px); }
            40% { transform: translate(3px, -3px); }
            60% { transform: translate(-3px, 3px); }
            80% { transform: translate(3px, -3px); }
            100% { transform: translate(0); }
        }

        h1::before,
        h1::after {
            content: "Sukii!";
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            color: red;
            background: black;
            overflow: hidden;
            clip: rect(0, 900px, 0, 0);
        }

        h1::before {
            left: -3px;
            text-shadow: -2px 0 red;
            animation: glitchTop 0.8s infinite;
        }

        h1::after {
            left: 3px;
            text-shadow: 2px 0 cyan;
            animation: glitchBottom 0.8s infinite;
        }

        @keyframes glitchTop {
            0% { clip: rect(0, 9999px, 0, 0); }
            50% { clip: rect(20px, 9999px, 60px, 0); }
            100% { clip: rect(0, 9999px, 0, 0); }
        }

        @keyframes glitchBottom {
            0% { clip: rect(0, 9999px, 0, 0); }
            50% { clip: rect(60px, 9999px, 100px, 0); }
            100% { clip: rect(0, 9999px, 0, 0); }
        }
    </style>
</head>
<body>
    <h1>Kontol</h1>
</body>
</html># New-project
