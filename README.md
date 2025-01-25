<html lang="it">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Il Tuo Sito</title>
    <link rel="stylesheet" href="styles.css">
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }

        .navbar {
            background-color: #888;
            padding: 1rem 0;
            position: fixed;
            top: 0;
            width: 100%;
            z-index: 1000;
        }

        .navbar ul {
            list-style: none;
            display: flex;
            justify-content: center;
            gap: 2rem;
            margin: 0;
            padding: 0;
        }

        .navbar ul li a {
            color: #fff;
            text-decoration: none;
            font-size: 1.2rem;
            font-weight: bold;
        }

        section {
            max-width: 1200px;
            margin: 5rem auto;
            padding: 1rem;
        }

        #home {
            text-align: center;
        }

        #home img {
            margin: 2rem 0;
            border-radius: 10px;
            width: 80%;
            max-width: 800px;
        }

        .social-links {
            margin-top: 1rem;
        }

        .social-links a {
            margin: 0 10px;
            text-decoration: none;
            font-size: 1.2rem;
            color: #222;
            font-weight: bold;
        }

        footer {
            background-color: #222;
            color: #fff;
            text-align: center;
            padding: 1rem 0;
            margin-top: 2rem;
        }

        footer img {
            margin-top: 10px;
            width: 50px;
        }

        .hidden {
            display: none;
        }
    </style>
    <script>
        function showSection(sectionId) {
            const sections = document.querySelectorAll('section');
            sections.forEach(section => {
                if (section.id === sectionId) {
                    section.classList.remove('hidden');
                } else {
                    section.classList.add('hidden');
                }
            });
        }

        document.addEventListener('DOMContentLoaded', () => {
            showSection('home'); // Mostra la home all'inizio
        });
    </script>
</head>
<body>
    <header class="navbar">
        <nav>
            <ul>
                <li><a href="#" onclick="showSection('home')">Home</a></li>
                <li><a href="#" onclick="showSection('shop')">Shop</a></li>
                <li><a href="#" onclick="showSection('about')">About</a></li>
                <li><a href="#" onclick="showSection('faq')">FAQ</a></li>
            </ul>
        </nav>
    </header>

    <section id="home">
        <h1>Benvenuto nel mio sito!</h1>
        <p>Qui troverai tutte le mie informazioni e i collegamenti ai miei social.</p>
        <img src="images/SFONDO_DESKTOP_2.jpg" alt="Immagine di Benvenuto">
        <div class="social-links">
            <a href="https://instagram.com/franzzinho.real?igsh=MTNoYng1OGVxaGQ2cQ==" target="_blank">Instagram</a>
            <a href="https://tiktok.com/@franzzinho.real?_t=8oTIcTP2vzN&_r=1" target="_blank">TikTok</a>
            <a href="https://open.spotify.com/playlist/6FufeeFmX0VN1OkYH06zI7?si=8954cbd0a899" target="_blank">Spotify</a>
            <a href="https://streamelements.com/franzzinho_tw/tip" target="_blank">Donazioni</a>
        </div>
    </section>

    <section id="shop" class="hidden">
        <h2>Shop</h2>
        <p>Acquista le mie magliette e altri prodotti qui!</p>
        <div class="products">
            <div class="product">
                <img src="images/SFONDO_DESKTOP_SFERA.jpg" alt="Prodotto 1">
                <p>Prodotto 1 - €100</p>
                <button>Acquista</button>
            </div>
            <div class="product">
                <img src="images/SFONDO_DESKTOP_3.jpg" alt="Prodotto 2">
                <p>Prodotto 2 - €200</p>
                <button>Acquista</button>
            </div>
        </div>
    </section>

    <section id="about" class="hidden">
        <h2>About</h2>
        <p>Scopri di più su di me e sulla mia storia.</p>
        <p>Mi chiamo Franzzinho e questo è il mio sito ufficiale per connettermi con i miei fan e supporter.</p>
    </section>

    <section id="faq" class="hidden">
        <h2>FAQ</h2>
        <p>Risposte alle domande più frequenti:</p>
        <ul>
            <li><strong>Come posso acquistare un prodotto?</strong> Puoi acquistarlo direttamente dalla sezione Shop.</li>
            <li><strong>Posso fare donazioni?</strong> Sì, cliccando sul link "Donazioni" nella sezione Home.</li>
            <li><strong>Dove posso ascoltare la tua musica?</strong> Su Spotify, il link è nella sezione Home.</li>
        </ul>
    </section>

    <footer>
        <p>© 2025 - SCANTOT NANO.</p>
        <img src="images/SFONDO_DESKTOP_SFERA.jpg" alt="Decorazione Footer">
    </footer>
</body>
</html>
