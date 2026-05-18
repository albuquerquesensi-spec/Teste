# Teste
<!DOCTYPE html><html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Para o Amor da Minha Vida</title>
  <style>
    body {
      margin: 0;
      font-family: 'Arial', sans-serif;
      background-color: #fff0f5;
      overflow-x: hidden;
    }
    header {
      background-color: #ff69b4;
      padding: 20px;
      text-align: center;
      color: white;
    }
    h1 {
      margin: 0;
    }
    .gallery {
      display: flex;
      flex-direction: column;
      align-items: center;
      padding: 20px;
    }
    .photo {
      margin: 20px 0;
      text-align: center;
    }
    .photo img {
      max-width: 90vw;
      height: auto;
      border-radius: 20px;
      box-shadow: 0px 0px 15px rgba(0,0,0,0.2);
    }
    .caption {
      margin-top: 10px;
      font-weight: bold;
      color: #333;
    }
    .heart {
      position: absolute;
      width: 20px;
      height: 20px;
      background: url('https://i.imgur.com/YpI4QUP.png') no-repeat center;
      background-size: contain;
      animation: fall 6s infinite;
      opacity: 0.8;
    }
    @keyframes fall {
      0% {
        transform: translateY(-100px);
        opacity: 1;
      }
      100% {
        transform: translateY(100vh);
        opacity: 0;
      }
    }
  </style>
</head>
<body>
  <header>
    <h1>Para a Minha Namorada Linda</h1>
    <p>Te amo com todo o meu coração. Essa página é só para você.</p>
  </header>
  <div class="gallery">
    <div class="photo">
      <img src="imagens/foto1.jpg" alt="Foto com filtro de cachorrinho">
      <div class="caption">Nosso amor e nossos sorrisos com filtro fofo!</div>
    </div>
    <div class="photo">
      <img src="imagens/foto2.jpg" alt="Beijo na praia">
      <div class="caption">Na praia, onde o amor é infinito como o mar.</div>
    </div>
    <div class="photo">
      <img src="imagens/foto3.jpg" alt="Abraço na igreja ou evento">
      <div class="caption">Momentos de emoção e fé juntos. Te amo demais!</div>
    </div>
  </div>  <!-- Corações caindo -->  <script>
    function criarCoracao() {
      const coracao = document.createElement("div");
      coracao.classList.add("heart");
      coracao.style.left = Math.random() * 100 + "vw";
      document.body.appendChild(coracao);
      setTimeout(() => coracao.remove(), 6000);
    }
    setInterval(criarCoracao, 500);
  </script>  <!-- Música de fundo -->  <audio autoplay loop>
    <source src="musica/alianca.mp3" type="audio/mpeg">
    Seu navegador não suporta o áudio :(
  </audio>
</body>
</html>
