<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Loja virtual de produtos domésticos com serviço de entrega.">
    <title>Loja Doméstica & Entregas</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            font-family: 'Arial', sans-serif;
            background-color: #f4f4f4;
            color: #333;
        }
        header {
            background-color: #4a4a4a;
            color: white;
            padding: 20px;
            text-align: center;
            font-size: 1.5rem;
        }
        h1 {
            font-size: 2.5rem;
            font-weight: bold;
        }
        nav {
            margin: 20px 0;
            display: flex;
            justify-content: center;
            gap: 20px;
        }
        nav a {
            text-decoration: none;
            color: #4a4a4a;
            font-weight: bold;
            font-size: 1.2rem;
        }
        nav a:hover {
            color: #ff6347; /* Tom criativo e moderno */
        }
        section {
            padding: 20px;
            text-align: center;
        }
        .product-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            margin-top: 20px;
        }
        .product {
            border: 2px solid #333;
            padding: 15px;
            border-radius: 10px;
            background-color: #fff;
        }
        .product img {
            max-width: 100%;
            border-radius: 10px;
        }
        .product h3 {
            margin: 10px 0;
            color: #ff6347;
        }
        .price {
            font-weight: bold;
            color: #333;
        }
        .add-to-cart-btn {
            background-color: #4a4a4a;
            color: white;
            padding: 10px;
            border: none;
            cursor: pointer;
            border-radius: 5px;
            margin-top: 10px;
            transition: background-color 0.3s ease;
        }
        .add-to-cart-btn:hover {
            background-color: #ff6347;
        }
        footer {
            background-color: #4a4a4a;
            color: white;
            text-align: center;
            padding: 20px;
            margin-top: 40px;
        }
        form {
            margin-top: 20px;
        }
        input, select {
            padding: 10px;
            margin: 10px 0;
            width: 100%;
            max-width: 400px;
        }
        button {
            background-color: #4a4a4a;
            color: white;
            padding: 10px;
            border: none;
            cursor: pointer;
            width: 100%;
            max-width: 400px;
            transition: background-color 0.3s;
        }
        button:hover {
            background-color: #ff6347;
        }
    </style>
</head>
<body>
    <header>
        <h1>Loja Doméstica & Entregas</h1>
        <nav>
            <a href="#produtos">Produtos</a>
            <a href="#entrega">Serviços de Entrega</a>
            <a href="#contato">Contato</a>
        </nav>
    </header>

    <section id="produtos">
        <h2>Produtos Domésticos</h2>
        <div class="product-grid">
            <div class="product">
                <img src="https://via.placeholder.com/200" alt="Produto 1">
                <h3>Panela de Pressão</h3>
                <p class="price">R$ 199,90</p>
                <button class="add-to-cart-btn">Adicionar ao Carrinho</button>
            </div>
            <div class="product">
                <img src="https://via.placeholder.com/200" alt="Produto 2">
                <h3>Aspirador de Pó</h3>
                <p class="price">R$ 299,90</p>
                <button class="add-to-cart-btn">Adicionar ao Carrinho</button>
            </div>
            <div class="product">
                <img src="https://via.placeholder.com/200" alt="Produto 3">
                <h3>Jogo de Talheres</h3>
                <p class="price">R$ 99,90</p>
                <button class="add-to-cart-btn">Adicionar ao Carrinho</button>
            </div>
        </div>
    </section>

    <section id="entrega">
        <h2>Serviço de Entrega</h2>
        <p>Oferecemos entrega rápida e segura para sua casa. Escolha a melhor opção para você:</p>
        <form action="#" method="post">
            <label for="nome">Nome:</label><br>
            <input type="text" id="nome" name="nome" required><br><br>
            <label for="endereco">Endereço:</label><br>
            <input type="text" id="endereco" name="endereco" required><br><br>
            <label for="opcao-entrega">Opção de Entrega:</label><br>
            <select id="opcao-entrega" name="opcao-entrega">
                <option value="rapida">Entrega Rápida (1-2 dias)</option>
                <option value="normal">Entrega Normal (3-5 dias)</option>
            </select><br><br>
            <button type="submit">Solicitar Entrega</button>
        </form>
    </section>

    <section id="contato">
        <h2>Entre em Contato</h2>
        <p>Para mais informações sobre nossos produtos e serviços, envie-nos uma mensagem.</p>
        <form action="#" method="post">
            <label for="email">E-mail:</label><br>
            <input type="email" id="email" name="email" required><br><br>
            <label for="mensagem">Mensagem:</label><br>
            <textarea id="mensagem" name="mensagem" rows="5" required></textarea><br><br>
            <button type="submit">Enviar Mensagem</button>
        </form>
    </section>

    <footer>
        <p>&copy; 2024 Loja Doméstica & Entregas. Todos os direitos reservados.</p>
    </footer>
</body>
</html>
