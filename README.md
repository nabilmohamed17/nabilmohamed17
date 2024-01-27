<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Pedido de Namoro</title>
  <style>
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      text-align: center;
      margin: 50px;
      background-color: #f5f5f5;
    }

    h1 {
      color: #e74c3c;
    }

    button {
      background-color: #2ecc71;
      color: white;
      padding: 15px 30px;
      font-size: 18px;
      cursor: pointer;
      margin: 20px;
      border: none;
      border-radius: 5px;
      transition: background-color 0.3s;
    }

    button:hover {
      background-color: #27ae60;
    }

    #mensagem {
      opacity: 0;
      margin-top: 20px;
      font-size: 18px;
      color: #333;
      transition: opacity 1s ease-in-out;
    }
  </style>
</head>
<body>

  <h1>Quer namorar comigo?</h1>

  <button id="btnSim" onclick="animacaoPedido()">Sim</button>

  <div id="mensagem">🎉 Parabéns! Vocês estão oficialmente namorando. Redirecionando... 🎉</div>

  <script>
    function animacaoPedido() {
      var btnSim = document.getElementById("btnSim");
      var mensagem = document.getElementById("mensagem");

      btnSim.style.display = "none";
      mensagem.style.opacity = 1;

      setTimeout(function() {
        window.location.href = "nova_pagina.html"; // Substitua "nova_pagina.html" pelo nome da sua nova página
      }, 3000); // Tempo em milissegundos antes do redirecionamento (aqui definido para 3 segundos)
    }
  </script>

</body>
</html>
