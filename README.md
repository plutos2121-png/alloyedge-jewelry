<!DOCTYPE html>
<html lang="sq">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ALLOYEDGE - Stoli për vajza të reja</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', 'Arial', sans-serif;
            background: linear-gradient(135deg, #fff9f9 0%, #fff0f5 100%);
            color: #4a4a4a;
            line-height: 1.6;
        }

        /* Gjethe dekorative */
        .leaf {
            position: fixed;
            opacity: 0.1;
            pointer-events: none;
            z-index: -1;
        }

        .leaf-1 {
            top: 50px;
            left: 20px;
            transform: rotate(-15deg);
            font-size: 100px;
        }

        .leaf-2 {
            bottom: 30px;
            right: 20px;
            transform: rotate(25deg);
            font-size: 120px;
        }

        .leaf-3 {
            top: 200px;
            right: 50px;
            transform: rotate(45deg);
            font-size: 80px;
        }

        /* Header dhe navigimi */
        header {
            background: rgba(255, 255, 255, 0.9);
            backdrop-filter: blur(10px);
            box-shadow: 0 2px 20px rgba(255, 182, 193, 0.2);
            position: sticky;
            top: 0;
            z-index: 100;
        }

        nav {
            max-width: 1200px;
            margin: 0 auto;
            padding: 1rem 2rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
        }

        .logo {
            display: flex;
            flex-direction: column;
            align-items: center;
            text-decoration: none;
        }

        .logo-icon {
            font-size: 2rem;
            filter: drop-shadow(0 4px 6px rgba(255, 105, 180, 0.3));
        }

        .logo-text {
            font-size: 1.8rem;
            font-weight: 700;
            letter-spacing: 3px;
            background: linear-gradient(45deg, #d44e6c, #f8a5b2);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .logo-sub {
            font-size: 0.9rem;
            color: #b76e79;
            letter-spacing: 4px;
        }

        .nav-links {
            display: flex;
            gap: 2.5rem;
            list-style: none;
        }

        .nav-links a {
            text-decoration: none;
            color: #6b4e5a;
            font-weight: 500;
            transition: all 0.3s ease;
            position: relative;
        }

        .nav-links a::after {
            content: '';
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 0;
            height: 2px;
            background: linear-gradient(90deg, #f8a5b2, #d44e6c);
            transition: width 0.3s ease;
        }

        .nav-links a:hover::after {
            width: 100%;
        }

        /* Hero seksioni */
        .hero {
            max-width: 1200px;
            margin: 4rem auto;
            padding: 0 2rem;
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 3rem;
            align-items: center;
        }

        .hero-content {
            animation: fadeInLeft 1s ease;
        }

        .hero-title {
            font-size: 3.5rem;
            line-height: 1.2;
            margin-bottom: 1rem;
            color: #4a2e35;
        }

        .hero-title span {
            background: linear-gradient(135deg, #d44e6c, #f8a5b2);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            display: inline-block;
        }

        .hero-description {
            font-size: 1.2rem;
            color: #6b5e64;
            margin-bottom: 2rem;
            max-width: 500px;
        }

        .btn {
            display: inline-block;
            padding: 1rem 2.5rem;
            background: linear-gradient(135deg, #f8a5b2, #d44e6c);
            color: white;
            text-decoration: none;
            border-radius: 50px;
            font-weight: 600;
            letter-spacing: 1px;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            border: none;
            cursor: pointer;
            box-shadow: 0 4px 15px rgba(212, 78, 108, 0.3);
        }

        .btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(212, 78, 108, 0.4);
        }

        .hero-image {
            text-align: center;
            animation: fadeInRight 1s ease;
        }

        .hero-image img {
            max-width: 100%;
            height: auto;
            border-radius: 30px;
            box-shadow: 0 20px 40px rgba(248, 165, 178, 0.2);
        }

        /* Produktet */
        .products {
            max-width: 1200px;
            margin: 6rem auto;
            padding: 0 2rem;
        }

        .section-title {
            text-align: center;
            font-size: 2.5rem;
            margin-bottom: 1rem;
            color: #4a2e35;
            position: relative;
        }

        .section-title::after {
            content: '✧';
            display: block;
            font-size: 2rem;
            color: #f8a5b2;
            margin-top: 0.5rem;
        }

        .product-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 2.5rem;
            margin-top: 3rem;
        }

        .product-card {
            background: white;
            border-radius: 20px;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(248, 165, 178, 0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            position: relative;
        }

        .product-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 40px rgba(248, 165, 178, 0.2);
        }

        .product-badge {
            position: absolute;
            top: 1rem;
            right: 1rem;
            background: linear-gradient(135deg, #f8a5b2, #d44e6c);
            color: white;
            padding: 0.3rem 1rem;
            border-radius: 25px;
            font-size: 0.8rem;
            font-weight: 600;
        }

        .product-image {
            height: 300px;
            background: linear-gradient(135deg, #fff0f5, #ffe4e9);
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .product-emoji {
            font-size: 5rem;
            filter: drop-shadow(0 4px 6px rgba(212, 78, 108, 0.3));
        }

        .product-info {
            padding: 1.5rem;
            text-align: center;
        }

        .product-title {
            font-size: 1.2rem;
            font-weight: 600;
            margin-bottom: 0.5rem;
            color: #4a2e35;
        }

        .product-price {
            color: #d44e6c;
            font-size: 1.3rem;
            font-weight: 700;
            margin-bottom: 1rem;
        }

        .product-description {
            color: #7a6a70;
            font-size: 0.9rem;
            margin-bottom: 1rem;
        }

        .btn-small {
            padding: 0.6rem 1.5rem;
            background: linear-gradient(135deg, #f8a5b2, #d44e6c);
            color: white;
            border: none;
            border-radius: 25px;
            cursor: pointer;
            font-size: 0.9rem;
            transition: transform 0.3s ease;
        }

        .btn-small:hover {
            transform: scale(1.05);
        }

        /* Përse të na zgjidhni */
        .features {
            max-width: 1200px;
            margin: 6rem auto;
            padding: 0 2rem;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
        }

        .feature {
            text-align: center;
            padding: 2rem;
            background: rgba(255, 255, 255, 0.7);
            backdrop-filter: blur(5px);
            border-radius: 20px;
            box-shadow: 0 5px 20px rgba(248, 165, 178, 0.1);
        }

        .feature-emoji {
            font-size: 2.5rem;
            margin-bottom: 1rem;
        }

        .feature-title {
            font-size: 1.2rem;
            font-weight: 600;
            color: #4a2e35;
            margin-bottom: 0.5rem;
        }

        .feature-description {
            color: #6b5e64;
            font-size: 0.95rem;
        }

        /* Footer */
        footer {
            background: rgba(255, 255, 255, 0.9);
            backdrop-filter: blur(10px);
            padding: 3rem 2rem 1rem;
            margin-top: 4rem;
        }

        .footer-content {
            max-width: 1200px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
        }

        .footer-section h3 {
            color: #4a2e35;
            margin-bottom: 1rem;
            font-size: 1.2rem;
        }

        .footer-section p, .footer-section a {
            color: #6b5e64;
            text-decoration: none;
            display: block;
            margin-bottom: 0.5rem;
            transition: color 0.3s ease;
        }

        .footer-section a:hover {
            color: #d44e6c;
        }

        .social-links {
            display: flex;
            gap: 1rem;
            font-size: 1.5rem;
        }

        .copyright {
            text-align: center;
            margin-top: 3rem;
            padding-top: 2rem;
            border-top: 1px solid rgba(212, 78, 108, 0.2);
            color: #6b5e64;
        }

        /* Animacionet */
        @keyframes fadeInLeft {
            from {
                opacity: 0;
                transform: translateX(-30px);
            }
            to {
                opacity: 1;
                transform: translateX(0);
            }
        }

        @keyframes fadeInRight {
            from {
                opacity: 0;
                transform: translateX(30px);
            }
            to {
                opacity: 1;
                transform: translateX(0);
            }
        }

        /* Responsive */
        @media (max-width: 768px) {
            nav {
                flex-direction: column;
                gap: 1rem;
            }

            .nav-links {
                gap: 1.5rem;
            }

            .hero {
                grid-template-columns: 1fr;
                text-align: center;
            }

            .hero-description {
                margin-left: auto;
                margin-right: auto;
            }

            .hero-title {
                font-size: 2.5rem;
            }
        }
    </style>
</head>
<body>
    <!-- Gjethe dekorative -->
    <div class="leaf leaf-1">🌿</div>
    <div class="leaf leaf-2">🍃</div>
    <div class="leaf leaf-3">🌱</div>

    <header>
        <nav>
            <a href="#" class="logo">
                <span class="logo-icon">🌿</span>
                <span class="logo-text">ALLOYEDGE</span>
                <span class="logo-sub">JEWELRY</span>
            </a>
            <ul class="nav-links">
                <li><a href="#ballina">Ballina</a></li>
                <li><a href="#produktet">Produktet</a></li>
                <li><a href="#rrethnesh">Rreth nesh</a></li>
                <li><a href="#kontakt">Kontakt</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section class="hero" id="ballina">
            <div class="hero-content">
                <h1 class="hero-title">
                    Shkëlqeni me<br>
                    <span>ALLOYEDGE</span>
                </h1>
                <p class="hero-description">
                    Stoli të punuara me dorë për vajzat që duan të shkëlqejnë. 
                    Çdo detaj është krijuar me dashuri për të nxjerrë në pah bukurinë tuaj të brendshme.
                </p>
                <a href="#produktet" class="btn">Shiko koleksionin</a>
            </div>
            <div class="hero-image">
                <div style="font-size: 15rem; line-height: 1;">💫</div>
            </div>
        </section>

        <section class="products" id="produktet">
            <h2 class="section-title">Produktet tona</h2>
            <div class="product-grid">
                <div class="product-card">
                    <span class="product-badge">Më të shitura</span>
                    <div class="product-image">
                        <span class="product-emoji">💍</span>
                    </div>
                    <div class="product-info">
                        <h3 class="product-title">Unazë me gjethe</h3>
                        <div class="product-price">€45</div>
                        <p class="product-description">Unazë argjendi me motiv gjetheje, e punuar me dorë</p>
                        <button class="btn-small">Blej tani</button>
                    </div>
                </div>

                <div class="product-card">
                    <div class="product-image">
                        <span class="product-emoji">📿</span>
                    </div>
                    <div class="product-info">
                        <h3 class="product-title">Byzylyk me zinxhir</h3>
                        <div class="product-price">€38</div>
                        <p class="product-description">Byzylyk i hollë me zinxhir të artë, për çdo ditë</p>
                        <button class="btn-small">Blej tani</button>
                    </div>
                </div>

                <div class="product-card">
                    <div class="product-image">
                        <span class="product-emoji">📿</span>
                    </div>
                    <div class="product-info">
                        <h3 class="product-title">Gjerdan me varëse</h3>
                        <div class="product-price">€52</div>
                        <p class="product-description">Gjerdan elegant me varëse në formë zemre</p>
                        <button class="btn-small">Blej tani</button>
                    </div>
                </div>

                <div class="product-card">
                    <div class="product-image">
                        <span class="product-emoji">💎</span>
                    </div>
                    <div class="product-info">
                        <h3 class="product-title">Vathë me perla</h3>
                        <div class="product-price">€41</div>
                        <p class="product-description">Vathë të vegjël me perla, për një look elegant</p>
                        <button class="btn-small">Blej tani</button>
                    </div>
                </div>
            </div>
        </section>

        <section class="features" id="rrethnesh">
            <div class="feature">
                <div class="feature-emoji">✋</div>
                <h3 class="feature-title">Punuara me dorë</h3>
                <p class="feature-description">Çdo stoli është punuar me kujdes dhe dashuri nga artizanët tanë</p>
            </div>
            <div class="feature">
                <div class="feature-emoji">🌿</div>
                <h3 class="feature-title">Materiale natyrale</h3>
                <p class="feature-description">Përdorim materiale cilësore që respektojnë natyrën</p>
            </div>
            <div class="feature">
                <div class="feature-emoji">🎁</div>
                <h3 class="feature-title">Paketim special</h3>
                <p class="feature-description">Çdo porosi vjen në një kuti të bukur, gati për dhuratë</p>
            </div>
            <div class="feature">
                <div class="feature-emoji">🚚</div>
                <h3 class="feature-title">Dërgesë falas</h3>
                <p class="feature-description">Për porosi mbi €50, dërgesa është falas në të gjithë Shqipërinë</p>
            </div>
        </section>
    </main>

    <footer id="kontakt">
        <div class="footer-content">
            <div class="footer-section">
                <h3>ALLOYEDGE</h3>
                <p>Stoli të punuara me dorë për vajzat që duan të shkëlqejnë. Çdo detaj është krijuar me dashuri.</p>
            </div>
            <div class="footer-section">
                <h3>Kontakt</h3>
                <p>📧 info@alloyedge.com</p>
                <p>📞 +355 69 123 4567</p>
                <p>📍 Tiranë, Shqipëri</p>
            </div>
            <div class="footer-section">
                <h3>Na ndiqni</h3>
                <div class="social-links">
                    <a href="#">📷</a>
                    <a href="#">📘</a>
                    <a href="#">📌</a>
                </div>
            </div>
        </div>
        <div class="copyright">
            <p>&copy; 2025 ALLOYEDGE. Të gjitha të drejtat e rezervuara.</p>
        </div>
    </footer>
</body>
</html>
