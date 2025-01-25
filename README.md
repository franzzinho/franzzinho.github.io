<!DOCTYPE html>
<html lang="it">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Barra Navigazione</title>
    <link rel="stylesheet" href="styles.css">
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }

        .navbar {
            background-color: #333;
            color: #fff;
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 0.5rem 1rem;
            position: fixed;
            top: 0;
            width: 100%;
            z-index: 1000;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
        }

        .navbar-logo {
            font-size: 1.5rem;
            font-weight: bold;
            color: #fff;
        }

        .navbar-logo img {
            height: 40px;
            margin-right: 10px;
        }

        .navbar-menu {
            display: flex;
            align-items: center;
            gap: 1.5rem;
        }

        .navbar-menu a {
            color: #fff;
            text-decoration: none;
            font-size: 1rem;
            font-weight: 500;
            transition: color 0.3s ease;
        }

        .navbar-menu a:hover {
            color: #f39c12;
        }

        .navbar-search {
            flex: 1;
            display: flex;
            justify-content: center;
        }

        .navbar-search input {
            width: 300px;
            padding: 0.5rem;
            border: none;
            border-radius: 20px;
            outline: none;
            font-size: 1rem;
            transition: box-shadow 0.3s ease;
        }

        .navbar-search input:focus {
            box-shadow: 0 0 8px rgba(243, 156, 18, 0.5);
        }

        .navbar-actions {
            display: flex;
            align-items: center;
            gap: 1rem;
        }

        .navbar-actions button,
        .navbar-actions a {
            background-color: #f39c12;
            color: #fff;
            border: none;
            border-radius: 20px;
            padding: 0.5rem 1rem;
            font-size: 0.9rem;
            font-weight: 500;
            cursor: pointer;
            text-decoration: none;
            transition: background-color 0.3s ease;
        }

        .navbar-actions button:hover,
        .navbar-actions a:hover {
            background-color: #e67e22;
        }

        .navbar-actions a {
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }

        .navbar-actions a svg {
            height: 20px;
            width: 20px;
        }

        .shop-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 1rem;
            padding: 2rem;
        }

        .product-card {
            background: #fff;
            border-radius: 10px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
            padding: 1rem;
            text-align: center;
        }

        .product-card img {
            max-width: 100%;
            border-radius: 10px;
            margin-bottom: 1rem;
        }

        .product-card h3 {
            font-size: 1.2rem;
            margin-bottom: 0.5rem;
        }

        .product-card p {
            font-size: 0.9rem;
            margin-bottom: 1rem;
        }

        .product-card button {
            background-color: #f39c12;
            color: #fff;
            border: none;
            padding: 0.5rem 1rem;
            border-radius: 20px;
            cursor: pointer;
            font-size: 0.9rem;
        }

        .product-card button:hover {
            background-color: #e67e22;
        }

        .cart-counter {
            position: relative;
        }

        .cart-counter::after {
            content: attr(data-count);
            position: absolute;
            top: -10px;
            right: -10px;
            background: red;
            color: white;
            border-radius: 50%;
            padding: 0.2rem 0.5rem;
            font-size: 0.8rem;
            font-weight: bold;
        }

        .faq-section {
            padding: 2rem;
        }

        .faq-item {
            margin-bottom: 1rem;
        }

        .faq-item h4 {
            margin: 0;
            font-size: 1.1rem;
        }

        .faq-item p {
            margin: 0.5rem 0 0;
            font-size: 0.9rem;
        }
    </style>
</head>
<body>
    <header class="navbar">
        <div class="navbar-logo">
            Franzzinho
        </div>
        <nav class="navbar-menu">
            <a href="#home">Home</a>
            <a href="#shop">Shop</a>
            <a href="#biglietti">Biglietti Parchi</a>
            <a href="#itinerari">Itinerari</a>
            <a href="#about">About</a>
            <a href="#faq">FAQ</a>
        </nav>
        <div class="navbar-search">
            <input type="text" placeholder="Cerca...">
        </div>
        <div class="navbar-actions">
            <a href="#accedi" class="login">
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 12H9m3 6V6" />
                </svg>
                Accedi
            </a>
            <a href="#carrello" class="cart cart-counter" data-count="0">
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 3h2l1 5h13l1-5h2m-4 10h-6m-2 0H5m7 0h7m-7-5H5m1 5l-2 9h16l-2-9" />
                </svg>
                Carrello
            </a>
        </div>
    </header>
    <main>
        <section id="home">
            <h1>Benvenuto nella Home!</h1>
            <p>Seguici sui nostri social:</p>
            <ul>
                <li><a href="https://facebook.com">Facebook</a></li>
                <li><a href="https://instagram.com">Instagram</a></li>
                <li><a href="https://twitter.com">Twitter</a></li>
            </ul>
        </section>
        <section id="shop" class="shop-container">
            <div class="product-card">
                <img src="maglietta.jpg" alt="Maglietta">
                <h3>Maglietta</h3>
                <p>€19.99</p>
                <button onclick="addToCart()">Aggiungi al Carrello</button>
            </div>
            <div class="product-card">
                <img src="felpa.jpg" alt="Felpa">
                <h3>Felpa</h3>
                <p>€39.99</p>
                <button onclick="addToCart()">Aggiungi al Carrello</button>
            </div>
            <div class="product-card">
                <img src="cappello.jpg" alt="Cappello">
                <h3>Cappello</h3>
                <p>€14.99</p>
                <button onclick="addToCart()">Aggiungi al Carrello</button>
            </div>
            <div class="product-card">
                <img src="portachiavi.jpg" alt="Portachiavi">
                <h3>Portachiavi</h3>
                <p>€9.99</p>
                <button onclick="addToCart()">Aggiungi al Carrello</button>
            </div>
        </section>
        <section id="faq" class="faq-section">
            <div class="faq-item">
                <h4>Sei davvero un GOAT?</h4>
                <p>È KIARO, IO SONO IL CAMPO BRANCO DI TUTTI I BROSKYS CRAZY PAZZI.</p>
            </div>
            <div class="faq-item">
                <h4>Posso fare donazioni?</h4>
                <p>Sì, cliccando sul link "Donazioni" nella sezione Home.</p>
            </div>
            <div class="faq-item">
                <h4>Dove posso ascoltare la tua musica?</h4>
                <p>Su Spotify, il link è nella sezione Home.</p>
            </div>
            <div class="faq-item">
                <h4>Posso contattarti direttamente?</h4>
                <p>Certo, tramite la sezione Contatti nella homepage.</p>
            </div>
            <div class="faq-item">
                <h4>Organizzi eventi?</h4>
                <p>Sì, puoi trovare i dettagli nella sezione Eventi.</p>
            </div>
            <div class="faq-item">
                <h4>Posso collaborare con te?</h4>
                <p>Sì, inviami un'email tramite la pagina Collaborazioni.</p>
            </div>
            <div class="faq-item">
                <h4>Ci sono promozioni attive?</h4>
                <p>Controlla nella sezione Shop per le ultime offerte.</p>
            </div>
            <div class="faq-item">
                <h4>Offri spedizioni internazionali?</h4>
                <p>Sì, spediamo in tutto il mondo.</p>
            </div>
            <div class="faq-item">
                <h4>Come posso seguire le tue news?</h4>
                <p>Iscriviti alla newsletter nella homepage.</p>
            </div>
            <div class="faq-item">
                <h4>Posso restituire un prodotto?</h4>
                <p>Sì, leggi la nostra politica di reso nella sezione Shop.</p>
            </div>
        </section>
    </main>
    <script>
        let cartCount = 0;

        function addToCart() {
            cartCount++;
            document.querySelector('.cart-counter').setAttribute('data-count', cartCount);
        }
    </script>
</body>
</html>
