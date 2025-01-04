# H.E.R.O-Voeux-2025
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Carte de Vœux 2025 - HERO</title>
    <style>
        body {
            margin: 0;
            font-family: 'Arial', sans-serif;
            background: linear-gradient(to bottom, #002a5e, #ffffff);
            color: #222;
            overflow: hidden;
        }

        .hero-logo {
            text-align: center;
            margin: 20px 0;
        }

        .hero-logo img {
            width: 300px;
            animation: fadeIn 3s ease-in-out;
        }

        @keyframes fadeIn {
            0% { opacity: 0; transform: scale(0.8); }
            100% { opacity: 1; transform: scale(1); }
        }

        .interactive-section {
            display: flex;
            justify-content: center;
            align-items: center;
            flex-wrap: wrap;
            gap: 20px;
            padding: 20px;
        }

        .button {
            background: #d32f2f;
            color: #fff;
            padding: 15px 25px;
            border: none;
            border-radius: 5px;
            font-size: 18px;
            cursor: pointer;
            box-shadow: 0 5px 10px rgba(0, 0, 0, 0.2);
            transition: transform 0.3s ease, background 0.3s ease;
        }

        .button:hover {
            transform: scale(1.1);
            background: #b71c1c;
        }

        .message-box {
            display: none;
            background: rgba(255, 255, 255, 0.9);
            padding: 20px;
            border-radius: 10px;
            text-align: center;
            font-size: 18px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
            animation: slideIn 1s ease forwards;
        }

        @keyframes slideIn {
            0% { opacity: 0; transform: translateY(30px); }
            100% { opacity: 1; transform: translateY(0); }
        }

        footer {
            text-align: center;
            padding: 10px;
            background: #002a5e;
            color: #fff;
            position: fixed;
            bottom: 0;
            width: 100%;
        }
    </style>
</head>
<body>

<div class="hero-logo">
    <img src="/mnt/data/Logo-HERO-light-x2.jpg.webp" alt="HERO Logo">
</div>

<div class="interactive-section">
    <button class="button" onclick="showMessage('Harmonie', 'En 2025, trouvez l’Harmonie dans chaque défi !')">Harmonie</button>
    <button class="button" onclick="showMessage('Engagement', 'Engagez-vous avec courage et passion.')">Engagement</button>
    <button class="button" onclick="showMessage('Relation', 'Tissez des Relations authentiques et durables.')">Relation</button>
    <button class="button" onclick="showMessage('Ouverture', 'Restez ouvert aux opportunités.')">Ouverture</button>
</div>

<div id="message-box" class="message-box"></div>

<footer>
    Bonne année 2025 - Soyez notre HÉROS !
</footer>

<script>
    function showMessage(title, message) {
        const messageBox = document.getElementById('message-box');
        messageBox.innerHTML = `<h2>${title}</h2><p>${message}</p>`;
        messageBox.style.display = 'block';

        setTimeout(() => {
            messageBox.style.display = 'none';
        }, 5000);
    }
</script>

</body>
</html>
