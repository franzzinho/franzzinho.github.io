<!DOCTYPE html>
<html lang="it">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Benvenuto su Franzzinho - il miglior shop online con contenuti esclusivi e tanto altro!">
    <meta name="keywords" content="Franzzinho, Shop, Video Exclusive, FAQ, GOAT">
    <meta name="author" content="Franzzinho">
    <title>Sito Web Professionale</title>
    <link rel="stylesheet" href="styles.css">
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha3/dist/css/bootstrap.min.css" rel="stylesheet">
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background-color: #333;
            color: #fff;
        }

        ![Image](https://github.com/user-attachments/assets/8a0d934b-84ad-40e3-a1dc-159354b8ceb6)

        .navbar {
            background-color: #222;
        }

        .navbar .nav-link {
            color: #f39c12 !important;
            margin-right: 1rem;
            transition: color 0.3s;
        }

        .navbar .nav-link:hover {
            color: #fff !important;
        }

        .hero {
            background: url('hero.jpg') no-repeat center center/cover;
            height: 60vh;
            display: flex;
            justify-content: center;
            align-items: center;
            color: #fff;
            text-shadow: 0 2px 5px rgba(0, 0, 0, 0.7);
        }

        .hero h1 {
            font-size: 3rem;
        }

        .section {
            padding: 4rem 2rem;
        }

        .section h2 {
            margin-bottom: 2rem;
            font-size: 2.5rem;
            color: #f39c12;
        }

        .video-exclusive {
            display: flex;
            flex-wrap: wrap;
            gap: 1rem;
        }

        .video-exclusive video {
            max-width: 100%;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(255, 255, 255, 0.2);
        }

        footer {
            background-color: #222;
            color: #fff;
            text-align: center;
            padding: 1rem 0;
            margin-top: 2rem;
        }

        footer a {
            color: #f39c12;
            text-decoration: none;
        }

        .cart-badge {
            background-color: #f39c12;
            color: white;
            border-radius: 50%;
            padding: 0.2rem 0.5rem;
            font-size: 0.8rem;
            position: relative;
            top: -10px;
            left: -10px;
        }

        .lang-selector {
            margin-left: 1rem;
            background-color: #222;
            color: #fff;
            border: 1px solid #f39c12;
        }

        .btn-warning {
            background-color: #f39c12;
            border: none;
        }

        .btn-warning:hover {
            background-color: #e67e22;
        }

        .card {
            background-color: #444;
            color: #fff;
            border: none;
        }

        .card img {
            border-radius: 10px;
        }

        .accordion-button {
            background-color: #444;
            color: #f39c12;
        }

        .accordion-button:not(.collapsed) {
            background-color: #555;
            color: #fff;
        }

        .accordion-body {
            background-color: #333;
            color: #fff;
        }
    </style>
</head>
<body>
    <nav class="navbar navbar-expand-lg navbar-dark">
        <div class="container">
            <a class="navbar-brand" href="#">Franzzinho</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto">
                    <li class="nav-item">
                        <a class="nav-link" href="#home">Home</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#shop">Shop</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#video-exclusive">Video Exclusive</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#faq">FAQ</a>
                    </li>
                    <li class="nav-item">
                        <select class="form-select lang-selector" aria-label="Lingua">
                            <option value="it" selected>IT</option>
                            <option value="en">EN</option>
                        </select>
                    </li>
                </ul>
            </div>
        </div>
    </nav>

    <header class="hero">
        <h1>Benvenuto su Franzzinho</h1>
    </header>

    <main>
        <section id="about" class="section">
            <div class="container">
                <h2>Chi Siamo</h2>
                <p>Franzzinho è il tuo punto di riferimento per articoli unici, contenuti esclusivi e tanto altro. Scopri il nostro shop e lasciati ispirare dai nostri video esclusivi. Siamo qui per offrirti il meglio!</p>
            </div>
        </section>

        <section id="shop" class="section">
            <div class="container">
                <h2>Shop</h2>
                <div class="row">
                    <div class="col-md-3">
                        <div class="card">
                            <img src="maglietta.jpg" class="card-img-top" alt="Maglietta">
                            <div class="card-body">
                                <h5 class="card-title">Maglietta</h5>
                                <p class="card-text">€19.99</p>
                                <button class="btn btn-warning">Aggiungi al Carrello <span class="cart-badge">1</span></button>
                            </div>
                        </div>
                    </div>
                    <div class="col-md-3">
                        <div class="card">
                            <img src="felpa.jpg" class="card-img-top" alt="Felpa">
                            <div class="card-body">
                                <h5 class="card-title">Felpa</h5>
                                <p class="card-text">€39.99</p>
                                <button class="btn btn-warning">Aggiungi al Carrello</button>
                            </div>
                        </div>
                    </div>
                    <div class="col-md-3">
                        <div class="card">
                            <img src="cappello.jpg" class="card-img-top" alt="Cappello">
                            <div class="card-body">
                                <h5 class="card-title">Cappello</h5>
                                <p class="card-text">€14.99</p>
                                <button class="btn btn-warning">Aggiungi al Carrello</button>
                            </div>
                        </div>
                    </div>
                    <div class="col-md-3">
                        <div class="card">
                            <img src="portachiavi.jpg" class="card-img-top" alt="Portachiavi">
                            <div class="card-body">
                                <h5 class="card-title">Portachiavi</h5>
                                <p class="card-text">€9.99</p>
                                <button class="btn btn-warning">Aggiungi al Carrello</button>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <section id="video-exclusive" class="section">
            <div class="container">
                <h2>Video Exclusive</h2>
                <div class="video-exclusive">
                    <video controls>
                        <source src="video1.mp4" type="video/mp4">
                        Il tuo browser non supporta il tag video.
                    </video>
                    <video controls>
                        <source src="video2.mp4" type="video/mp4">
                        Il tuo browser non supporta il tag video.
                    </video>
                </div>
            </div>
        </section>

        <section id="faq" class="section">
            <div class="container">
                <h2>FAQ</h2>
                <div class="accordion" id="faqAccordion">
                    <div class="accordion-item">
                        <h2 class="accordion-header" id="headingOne">
                            <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne">
                                Sei davvero un GOAT?
                            </button>
                        </h2>
                        <div id="collapseOne" class="accordion-collapse collapse">
                            <div class="accordion-body">
                                È KIARO, IO SONO IL CAMPO BRANCO DI TUTTI I BROSKYS CRAZY PAZZI.
                            </div>
                        </div>
                    </div>
                    <!-- Altre FAQ qui -->
                </div>
            </div>
        </section>
    </main>

    <footer>
        <p>© 2025 Franzzinho. Tutti i diritti riservati. <a href="#">Privacy</a> | <a href="#">Termini</a></p>
    </footer>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
