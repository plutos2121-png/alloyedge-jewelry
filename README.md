<!DOCTYPE html>
<html lang="sq">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>ALLOYEDGE - Jewelry</title>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&family=Playfair+Display:wght@500;700&display=swap" rel="stylesheet">

<style>

body{
    margin:0;
    font-family:'Poppins', sans-serif;
    background: linear-gradient(to bottom, #fce4ec, #f8bbd0);
    color:#444;
}

header{
    background: rgba(255,255,255,0.85);
    backdrop-filter: blur(10px);
    padding:20px 50px;
    display:flex;
    justify-content:space-between;
    align-items:center;
    position:fixed;
    width:100%;
    z-index:1000;
}

header img{
    height:60px;
}

nav a{
    margin-left:25px;
    text-decoration:none;
    color:#b76e79;
    font-weight:500;
    transition:0.3s;
}

nav a:hover{
    color:#8e3b46;
}

.hero{
    height:100vh;
    display:flex;
    align-items:center;
    justify-content:center;
    text-align:center;
    background-image: url('logo.png');
    background-size:cover;
    background-position:center;
    position:relative;
}

.hero::before{
    content:"";
    position:absolute;
    top:0;
    left:0;
    width:100%;
    height:100%;
    background:rgba(255,255,255,0.7);
}

.hero-content{
    position:relative;
    max-width:600px;
}

.hero h1{
    font-family:'Playfair Display', serif;
    font-size:48px;
    color:#b76e79;
}

.hero p{
    font-size:18px;
    margin:20px 0;
}

.btn{
    background:#b76e79;
    color:white;
    padding:12px 30px;
    border:none;
    border-radius:30px;
    cursor:pointer;
    font-size:16px;
    transition:0.3s;
}

.btn:hover{
    background:#8e3b46;
}

.section{
    padding:80px 10%;
    text-align:center;
}

.section h2{
    font-family:'Playfair Display', serif;
    font-size:36px;
    color:#b76e79;
}

.products{
    display:grid;
    grid-template-columns:repeat(auto-fit, minmax(250px,1fr));
    gap:30px;
    margin-top:40px;
}

.card{
    background:white;
    border-radius:20px;
    padding:20px;
    box-shadow:0 10px 30px rgba(0,0,0,0.1);
    transition:0.4s;
}

.card:hover{
    transform:translateY(-10px);
}

.card img{
    width:100%;
    border-radius:15px;
}

.card h3{
    color:#b76e79;
}

footer{
    background:#b76e79;
    color:white;
    text-align:center;
    padding:30px;
}

</style>
</head>

<body>

<header>
    <img src="logo.png" alt="ALLOYEDGE Logo">
    <nav>
        <a href="#">Ballina</a>
        <a href="#produkte">Produktet</a>
        <a href="#rreth">Rreth Nesh</a>
        <a href="#kontakt">Kontakt</a>
    </nav>
</header>

<section class="hero">
    <div class="hero-content">
        <h1>Elegancë për çdo vajzë ✨</h1>
        <p>Bizhuteri delikate, moderne dhe plot shkëlqim për stilin tënd unik.</p>
        <button class="btn">Shiko Koleksionin</button>
    </div>
</section>

<section class="section" id="produkte">
    <h2>Koleksioni Ynë</h2>
    <div class="products">
        <div class="card">
            <img src="https://via.placeholder.com/300x300" alt="">
            <h3>Vathë Elegant</h3>
            <p>19.99€</p>
        </div>

        <div class="card">
            <img src="https://via.placeholder.com/300x300" alt="">
            <h3>Qafore Delikate</h3>
            <p>24.99€</p>
        </div>

        <div class="card">
            <img src="https://via.placeholder.com/300x300" alt="">
            <h3>Unazë Minimaliste</h3>
            <p>17.99€</p>
        </div>
    </div>
</section>

<section class="section" id="rreth">
    <h2>Rreth ALLOYEDGE</h2>
    <p>ALLOYEDGE është një brand modern për vajza të reja që duan stil, elegancë dhe shkëlqim në çdo moment. Çdo bizhuteri është zgjedhur me kujdes për të reflektuar bukurinë dhe vetëbesimin.</p>
</section>

<section class="section" id="kontakt">
    <h2>Na Kontakto</h2>
    <p>Email: info@alloyedge.com</p>
    <p>Instagram: @alloyedge</p>
</section>

<footer>
    © 2026 ALLOYEDGE Jewelry | Të gjitha të drejtat e rezervuara
</footer>

</body>
</html>
