<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Aplicativo Simples</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
    }
    
    input[type="text"] {
      width: 50%;
      height: 30px;
      font-size: 18px;
      padding: 10px;
      border: 1px solid #ccc;
    }
    
    button {
      width: 20%;
      height: 30px;
      font-size: 18px;
      background-color: #4CAF50;
      color: #fff;
      border: none;
      cursor: pointer;
    }
    
    button:hover {
      background-color: #3e8e41;
    }
  </style>
</head>
<body>
  <h1 id="titulo">Bem-vindo!</h1>
  <input id="nome" type="text" placeholder="Digite seu nome">
  <button id="botao">Enviar</button>
  <p id="mensagem"></p>
  
  <script>
    document.getElementById("botao").addEventListener("click", function() {
      var nome = document.getElementById("nome").value;
      if (nome !== "") {
        document.getElementById("titulo").textContent = `Olá, ${nome}!`;
        document.getElementById("mensagem").textContent = "Seja bem-vindo!";
      } else {
        alert("Por favor, insira seu nome.");
      }
    });
  </script>
</body>
</html>
