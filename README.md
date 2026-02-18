<!DOCTYPE html>
<html lang="sq">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ALLOYEDGE ✿ Stoli për vajza të reja</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', 'Arial', sans-serif;
            background: linear-gradient(135deg, #fff5f7 0%, #f0f7f0 100%);
            min-height: 100vh;
            color: #4a5a4a;
            line-height: 1.6;
        }

        /* Gjethe dekorative */
        .leaf-bg {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: -1;
            opacity: 0.15;
            background-image: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100" width="100" height="100"><path d="M50,20 Q60,10 70,20 Q80,30 70,40 Q60,50 50,40 Q40,30 50,20" fill="%23d44e6c"/><path d="M30,50 Q40,40 50,50 Q60,60 50,70 Q40,80 30,70 Q20,60 30,50" fill="%2389c989"/></svg>');
            background-repeat: repeat;
            background-size: 100px 100px;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }

        /* Header */
        header {
            text-align: center;
            padding: 40px 20px 20px;
            animation: fadeInDown 1s ease;
        }

        .logo-icon {
            font-size: 3.5rem;
            display: block;
            margin-bottom: 5px;
            filter: drop-shadow(0 4px 10px rgba(212, 78, 108, 0.3));
        }

        h1 {
            font-size: 3.5rem;
            font-weight: 700;
            letter-spacing: 3px;
            background: linear-gradient(45deg, #d44e6c, #89c989);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            line-height: 1.2;
            text-shadow: 2px 2px 10px rgba(255, 255, 255, 0.5);
        }

        .subtitle {
            font-size: 1.2rem;
            color: #89a989;
            letter-spacing: 3px;
            margin-top: 5px;
            font-weight: 300;
        }

        /* Nav */
        nav {
            display: flex;
            justify-content: center;
            gap: 30px;
            margin: 30px 0;
            flex-wrap: wrap;
        }

        nav a {
            text-decoration: none;
            color: #6b8e6b;
            font-weight: 500;
            padding: 8px 20px;
            border-radius: 30px;
            background: rgba(255, 255, 255, 0.7);
            backdrop-filter: blur(5px);
            transition: all 0.3s ease;
            border: 1px solid rgba(137, 201, 137, 0.3);
        }

        nav a:hover {
            background: #89c989;
            color: white;
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(137, 201, 137, 0.4);
        }

        /* Hero Section */
        .hero {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 40px;
            align-items: center;
            margin: 60px 0;
            background: rgba(255, 255, 255, 0.5);
            backdrop-filter: blur(5px);
            border-radius: 40px;
            padding: 40px;
            box-shadow: 0 15px 30px rgba(212, 78, 108, 0.1);
            border: 1px solid rgba(255, 255, 255, 0.8);
            animation: fadeIn 1.5s ease;
        }

        .hero-text h2 {
            font-size: 2.5rem;
            color: #d44e6c;
            margin-bottom: 20px;
        }

        .hero-text p {
            font-size: 1.1rem;
            color: #5a7a5a;
            margin-bottom: 30px;
        }

        .btn {
            display: inline-block;
            padding: 12px 35px;
            background: linear-gradient(135deg, #f8c3d0, #89c989);
            color: white;
            text-decoration: none;
            border-radius: 50px;
            font-weight: 600;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            border: none;
            cursor: pointer;
            box-shadow: 0 4px 15px rgba(137, 201, 137, 0.3);
        }

        .btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(212, 78, 108, 0.3);
        }

        .hero-image {
            text-align: center;
        }

        .hero-emoji {
            font-size: 10rem;
            line-height: 1;
            filter: drop-shadow(0 10px 20px rgba(212, 78, 108, 0.3));
            animation: float 6s ease-in-out infinite;
        }

        /* Produktet */
        .products {
            margin: 80px 0;
        }

        .section-title {
            text-align: center;
            font-size: 2.2rem;
            margin-bottom: 40px;
            color: #5a7a5a;
            position: relative;
        }

        .section-title::after {
            content: '✿';
            display: block;
            font-size: 2rem;
            color: #d44e6c;
            margin-top: 10px;
        }

        .product-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 25px;
        }

        .product-card {
            background: white;
            border-radius: 30px;
            padding: 20px;
            text-align: center;
            box-shadow: 0 10px 25px rgba(212, 78, 108, 0.1);
            transition: all 0.3s ease;
            border: 2px solid transparent;
            animation: fadeInUp 1s ease;
        }

        .product-card:hover {
            transform: translateY(-10px);
            border-color: #89c989;
            box-shadow: 0 20px 35px rgba(137, 201, 137, 0.2);
        }

        .product-emoji {
            font-size: 4rem;
            margin-bottom: 15px;
        }

        .product-card h3 {
            color: #d44e6c;
            margin-bottom: 10px;
        }

        .product-price {
            color: #89c989;
            font-size: 1.3rem;
            font-weight: bold;
            margin: 10px 0;
        }

        .product-desc {
            color: #8a9a8a;
            font-size: 0.9rem;
            margin-bottom: 15px;
        }

        .btn-small {
            padding: 8px 25px;
            background: linear-gradient(135deg, #89c989, #f8c3d0);
            border: none;
            border-radius: 25px;
            color: white;
            cursor: pointer;
            transition: transform 0.3s ease;
        }

        .btn-small:hover {
            transform: scale(1.05);
        }

        /* Kontakt Seksioni */
        .contact {
            background: rgba(255, 255, 255, 0.7);
            backdrop-filter: blur(5px);
            border-radius: 40px;
            padding: 50px 30px;
            margin: 60px 0;
            text-align: center;
            border: 1px solid rgba(137, 201, 137, 0.3);
            animation: fadeIn 1s ease;
        }

        .contact h2 {
            font-size: 2.2rem;
            color: #5a7a5a;
            margin-bottom: 15px;
        }

        .contact p {
            color: #7a9a7a;
            margin-bottom: 40px;
            font-size: 1.1rem;
        }

        .social-links {
            display: flex;
            justify-content: center;
            gap: 40px;
            flex-wrap: wrap;
        }

        .social-item {
            display: flex;
            flex-direction: column;
            align-items: center;
            text-decoration: none;
            transition: transform 0.3s ease;
        }

        .social-item:hover {
            transform: translateY(-10px);
        }

        .social-icon {
            width: 80px;
            height: 80px;
            background: linear-gradient(135deg, #f8c3d0, #89c989);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 15px;
            font-size: 2rem;
            color: white;
            box-shadow: 0 10px 20px rgba(212, 78, 108, 0.2);
        }

        .social-handle {
            font-size: 1.1rem;
            color: #5a7a5a;
            font-weight: 500;
        }

        .instagram .social-handle {
            color: #d44e6c;
        }

        .tiktok .social-handle {
            color: #89c989;
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 30px 20px;
            color: #8a9a8a;
            border-top: 2px solid rgba(137, 201, 137, 0.3);
            margin-top: 40px;
        }

        /* Animacionet */
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        @keyframes fadeInDown {
            from {
                opacity: 0;
                transform: translateY(-30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        @keyframes float {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-20px); }
        }

        /* Responsive */
        @media (max-width: 768px) {
            h1 {
                font-size: 2.5rem;
            }

            .hero {
                grid-template-columns: 1fr;
                text-align: center;
                padding: 30px;
            }

            .hero-image {
                order: -1;
            }

            .hero-emoji {
                font-size: 7rem;
            }

            .social-icon {
                width: 60px;
                height: 60px;
                font-size: 1.5rem;
            }

            .social-links {
                gap: 20px;
            }
        }
    </style>
</head>
<body>
    <div class="leaf-bg"></div>

    <div class="container">
        <header>
            <span class="logo-icon">🌿✨</span>
            <h1>ALLOYEDGE</h1>
            <div class="subtitle">JEWELRY</div>
        </header>

        <nav>
            <a href="#ballina">Ballina</a>
            <a href="#produktet">Produktet</a>
            <a href="#rrethnesh">Rreth nesh</a>
            <a href="#kontakt">Kontakt</a>
        </nav>

        <section class="hero" id="ballina">
            <div class="hero-text">
                <h2>Shkëlqeni me ALLOYEDGE</h2>
                <p>Stoli të punuara me dorë për vajzat që duan të shkëlqejnë. Çdo detaj është krijuar me dashuri për të nxjerrë në pah bukurinë tuaj të brendshme.</p>
                <a href="#produktet" class="btn">Shiko koleksionin</a>
            </div>
            <div class="hero-image">
                <div class="hero-emoji">💫</div>
            </div>
        </section>

        <section class="products" id="produktet">
            <h2 class="section-title">Produktet tona</h2>
            <div class="product-grid">
                <div class="product-card">
                    <div class="product-emoji">💍</div>
                    <h3>Unazë me gjethe</h3>
                    <div class="product-price">€45</div>
                    <p class="product-desc">Unazë argjendi me motiv gjetheje</p>
                    <button class="btn-small">Blej tani</button>
                </div>

                <div class="product-card">
                    <div class="product-emoji">📿</div>
                    <h3>Byzylyk me zinxhir</h3>
                    <div class="product-price">€38</div>
                    <p class="product-desc">Byzylyk i hollë me zinxhir të artë</p>
                    <button class="btn-small">Blej tani</button>
                </div>

                <div class="product-card">
                    <div class="product-emoji">📿</div>
                    <h3>Gjerdan me varëse</h3>
                    <div class="product-price">€52</div>
                    <p class="product-desc">Gjerdan elegant me varëse zemre</p>
                    <button class="btn-small">Blej tani</button>
                </div>

                <div class="product-card">
                    <div class="product-emoji">💎</div>
                    <h3>Vathë me perla</h3>
                    <div class="product-price">€41</div>
                    <p class="product-desc">Vathë të vegjël me perla</p>
                    <button class="btn-small">Blej tani</button>
                </div>
            </div>
        </section>

        <section class="contact" id="kontakt">
            <h2>Na kontaktoni</h2>
            <p>Na ndiqni në rrjetet sociale për të parë modelet më të reja</p>
            
            <div class="social-links">
                <a href="https://instagram.com/alloyedge.jewelry" target="_blank" class="social-item instagram">
                    <div class="social-icon">📷</div>
                    <span class="social-handle">@alloyedge.jewelry</span>
                </a>

                <a href="https://tiktok.com/@alloyedge.jewelry" target="_blank" class="social-item tiktok">
                    <div class="social-icon">🎵</div>
                    <span class="social-handle">@alloyedge.jewelry</span>
                </a>
            </div>

            <div style="margin-top: 30px; color: #89a989;">
                <p>📧 Email: info@alloyedge.com</p>
                <p>📞 Tel: +355 69 123 4567</p>
            </div>
        </section>

        <footer>
            <p>© 2025 ALLOYEDGE JEWELRY. Të gjitha të drejtat e rezervuara.</p>
            <p style="font-size: 0.9rem; margin-top: 10px;">✨ Krijuar me dashuri për vajzat shqiptare ✨</p>
        </footer>
    </div>
</body>
</html>
