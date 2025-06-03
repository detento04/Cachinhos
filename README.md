
<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Feliz Aniversário, Amor!</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Great+Vibes&family=Poppins:wght@300;500;700&display=swap" rel="stylesheet">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Poppins', sans-serif;
      background: linear-gradient(120deg, #ffe6f0 0%, #fffbe6 100%);
      color: #333;
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
      flex-direction: column;
      padding: 20px;
    }

    h1 {
      font-family: 'Great Vibes', cursive;
      font-size: 3em;
      color: #e91e63;
      margin-bottom: 10px;
    }

    .mensagem {
      font-size: 1.1em;
      background-color: rgba(255,255,255,0.8);
      padding: 20px;
      border-radius: 12px;
      box-shadow: 0 8px 20px rgba(0,0,0,0.1);
      max-width: 800px;
      text-align: center;
      margin-bottom: 30px;
    }

    .galeria {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
      width: 100%;
      max-width: 900px;
      margin-bottom: 40px;
    }

    .galeria img {
      width: 100%;
      border-radius: 15px;
      object-fit: cover;
      box-shadow: 0 5px 15px rgba(0,0,0,0.1);
      transition: transform 0.3s ease;
    }

    .galeria img:hover {
      transform: scale(1.03);
    }

    .botao-musica {
      background-color: #e91e63;
      color: white;
      border: none;
      padding: 12px 30px;
      font-size: 1em;
      border-radius: 25px;
      cursor: pointer;
      transition: background 0.3s ease;
    }

    .botao-musica:hover {
      background-color: #d81b60;
    }
  </style>
</head>
<body>
  <h1>Feliz Aniversário, Amor!</h1>

  <div class="mensagem">
    Hoje celebramos mais um ano da pessoa que ilumina meus dias. <br>
    Sua alegria, sua força e seu sorriso fazem da minha vida um lugar melhor. <br>
    Obrigado por ser quem é, por estar ao meu lado, e por compartilhar tanto amor. <br>
    Te amo demais. Feliz aniversário! 💖
  </div>

  <div class="galeria">
    <img src="foto1.jpg" alt="Foto 1">
    <img src="foto2.jpg" alt="Foto 2">
    <img src="foto3.jpg" alt="Foto 3">
  </div>

  <button class="botao-musica" onclick="tocarMusica()" id="btnMusica">🎵 Tocar Música</button>
  <audio id="musica" src="https://dl.sndup.net/krk6/lagrimas-do-bacu.mp3" loop></audio>

  <script>
    const musica = document.getElementById('musica');
    const btn = document.getElementById('btnMusica');

    function tocarMusica() {
      if (musica.paused) {
        musica.play();
        btn.textContent = '⏸️ Pausar Música';
      } else {
        musica.pause();
        btn.textContent = '🎵 Tocar Música';
      }
    }
  </script>
</body>
</html>
