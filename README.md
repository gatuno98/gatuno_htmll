<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <title>Alerta Gatuno</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      background: black;
      overflow: hidden;
      animation: fundo 1s infinite alternate;
    }

    @keyframes fundo {
      0% { background-color: black; }
      100% { background-color: darkred; }
    }

    .aviso {
      position: absolute;
      top: 40%;
      left: 50%;
      transform: translate(-50%, -50%);
      color: red;
      font-size: 4em;
      font-family: 'Arial Black', sans-serif;
      text-align: center;
      animation: piscar 1s infinite;
      text-shadow: 2px 2px 10px #ff0000;
    }

    @keyframes piscar {
      0%, 50%, 100% { opacity: 1; }
      25%, 75% { opacity: 0; }
    }

    .botao-falso {
      position: absolute;
      bottom: 100px;
      left: 50%;
      transform: translateX(-50%);
      padding: 20px 40px;
      font-size: 1.5em;
      background: #ff0000;
      color: white;
      border: none;
      cursor: pointer;
      font-family: 'Arial Black', sans-serif;
      box-shadow: 0 0 20px red;
      transition: 0.3s;
    }

    .botao-falso:hover {
      background: black;
      color: red;
    }
  </style>
</head>
<body>
  <div class="aviso">
    VOCÊ ESTÁ SENDO HACKEADO PELO GATUNO!
  </div>
  <button class="botao-falso" onclick="troll()">Fechar</button>

  <audio autoplay loop>
    <source src="https://www.myinstants.com/media/sounds/windows-xp-error.mp3" type="audio/mpeg">
    Seu navegador não suporta áudio.
  </audio>

  <script>
    function troll() {
      alert("É tarde demais... O Gatuno já entrou no seu sistema 😈");
    }
  </script>
</body>
</html>
