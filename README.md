<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Para Anna</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #ffe4e1;
            background-image: url('https://www.transparenttextures.com/patterns/flower-power.png'); /* Padrão floral sutil */
            background-size: cover;
            background-attachment: fixed;
            color: #333;
            text-align: center;
            padding: 50px;
            margin: 0;
            overflow: hidden; /* Evita barras de rolagem indesejadas */
        }
        h1 {
            color: #ff1493;
            font-size: 2.5em;
            margin-bottom: 20px;
            opacity: 0;
            animation: fadeIn 2s forwards;
        }
        .container {
            max-width: 600px;
            margin: 0 auto;
            padding: 20px;
            border: 2px solid #ff1493;
            border-radius: 15px;
            background-color: #fff;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            position: relative;
            transform: scale(0);
            animation: scaleIn 1s forwards 0.5s;
        }
        .heart {
            font-size: 2.5em;
            color: #ff1493;
            animation: rotateHeart 2s infinite linear;
        }
        footer {
            margin-top: 30px;
            font-size: 0.9em;
            color: #ff1493;
            opacity: 0;
            animation: fadeIn 3s forwards 2s;
        }
        #message {
            display: none;
            margin-top: 20px;
            font-size: 1.2em;
            color: #333;
        }
        .button {
            background-color: #ff1493;
            color: white;
            border: none;
            padding: 15px 30px;
            font-size: 1.2em;
            cursor: pointer;
            border-radius: 5px;
            transition: background-color 0.3s ease, transform 0.3s ease;
            margin-top: 20px;
            opacity: 0;
            animation: fadeIn 2s forwards 1.5s;
        }
        .button:hover {
            background-color: #ff69b4;
            transform: scale(1.1);
        }
        
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        
        @keyframes scaleIn {
            from { transform: scale(0); }
            to { transform: scale(1); }
        }
        
        @keyframes rotateHeart {
            from { transform: rotate(0deg); }
            to { transform: rotate(360deg); }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Para a minha querida Anna</h1>
        <button class="button" onclick="revealMessage()">Clique aqui para ver a mensagem</button>
        <div id="message">
            <p>
                Minha amada Anna,<br>
                Desde o momento em que nos conhecemos, você trouxe uma luz incrível para minha vida. Sua presença ilumina meus dias e seu sorriso é a razão do meu contentamento.
            </p>
            <p>
                Quero que saiba o quanto você significa para mim. Cada momento ao seu lado é um presente, e eu sou eternamente grato por ter você como minha namorada. A forma como você entende, apoia e ama me faz sentir a pessoa mais especial do mundo.
            </p>
            <p>
                Com você, tudo parece mais bonito e mais significativo. Eu te amo mais do que as palavras podem expressar e amo esse bundão tambémm.
            </p>
            <p class="heart">❤️</p>
            <p>
                Com todo o meu amor,<br>
                Kauã Lindao
            </p>
        </div>
    </div>
    <footer>
        Feito com amor, para Anna.
    </footer>
    <script>
        function revealMessage() {
            document.getElementById('message').style.display = 'block';
        }
    </script>
</body>
</html>
