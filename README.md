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
</html

  margin-bottom: 20px;
}

.card-container {
  display: flex;
  flex-direction: column;
  gap: 20px;
}

.card {
  background-color: #ffffff;
  border: 2px solid #d4a6ff;
  border-radius: 15px;
  padding: 20px;
  box-shadow: 0 4px 8px rgba(100, 0, 160, 0.1);
  transition: transform 0.2s;
}

.card:hover {
  transform: translateY(-5px);
}

.card img {
  width: 100%;
  border-radius: 10px;
}

.card h3 {
  margin-top: 10px;
  color: #5e0b86;
}

.card span {
  display: block;
  margin-top: 10px;
  font-weight: bold;
  color: #7a1ea1;
}

/* Pix */
.pix-section {
  background-color: #efdbff;
  padding: 30px 20px;
  text-align: center;
}

.pix-section h2 {
  color: #5e0b86;
  margin-bottom: 10px;
}

.pix-section button {
  background-color: #5e0b86;
  color: white;
  border: none;
  padding: 12px 20px;
  font-size: 1em;
  border-radius: 25px;
  cursor: pointer;
  margin-top: 10px;
}

.pix-section button:hover {
  background-color: #7a1ea1;
}

#msg-copiado {
  margin-top: 10px;
  color: green;
  font-weight: bold;
}

/* Rodapé */
footer {
  background-color: #4d076b;
  color: white;
  text-align: center;
  padding: 20px;
  margin-top: 40px;
}

/* Media Queries para telas maiores */
@media (min-width: 600px) {
  nav ul {
    display: flex;
    justify-content: center;
    gap: 20px;
    margin-top: 0;
  }

  nav ul li {
    margin: 0;
  }

  .banner h2 {
    font-size: 2.2em;
  }

  .produtos h2 {
    font-size: 2em;
  }

  .card-container {
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: center;
  }

  .card {
    width: 250px;
  }
}

@media (min-width: 900px) {
  header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    text-align: left;
  }

  header h1 {
    font-size: 2em;
  }
}


