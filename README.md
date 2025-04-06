<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Açaí do César</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <header>
    <h1>Açaí do César</h1>
    <nav>
      <ul>
        <li><a href="#">Início</a></li>
        <li><a href="#produtos">Produtos</a></li>
        <li><a href="#contato">Contato</a></li>
      </ul>
    </nav>
  </header>

  <section class="banner">
    <h2>Refresque-se com o melhor Açaí da cidade!</h2>
    <p>Pedidos online com entrega rápida</p>
    <a href="#produtos" class="btn">Ver Produtos</a>
  </section>

  <section id="produtos" class="produtos">
    <h2>Nossos Açaís</h2>
    <div class="card-container">
      <div class="card">
        <img src="https://i.imgur.com/jOeKpWn.png" alt="Açaí Tradicional" />
        <h3>Açaí Tradicional</h3>
        <p>300ml com banana e granola</p>
        <span>R$ 14,90</span>
      </div>
      <div class="card">
        <img src="https://i.imgur.com/fOKT9w7.png" alt="Açaí com Leite Ninho" />
        <h3>Açaí com Leite Ninho</h3>
        <p>400ml com leite condensado</p>
        <span>R$ 17,90</span>
      </div>
      <div class="card">
        <img src="https://i.imgur.com/UQ7RZIM.png" alt="Açaí Power" />
        <h3>Açaí Power</h3>
        <p>500ml com tudo que você ama</p>
        <span>R$ 22,90</span>
      </div>
    </div>
  </section>

  <section class="pix-section">
    <h2>Pagamento via Pix</h2>
    <p>Chave Pix: <strong>cesarsouuza01@gmail.com</strong></p>
    <button onclick="copiarPix()">Copiar chave Pix</button>
    <p id="msg-copiado"></p>
  </section>

  <footer id="contato">
    <p>&copy; 2025 Açaí do César - Todos os direitos reservados</p>
    <p>Contato: (99) 99999-9999</p>
  </footer>

  <script>
    function copiarPix() {
      const chave = "cesarsouuza01@gmail.com";
      navigator.clipboard.writeText(chave).then(() => {
        document.getElementById("msg-copiado").innerText = "Chave Pix copiada!";
      });
    }
  </script>
</body>
</html>


