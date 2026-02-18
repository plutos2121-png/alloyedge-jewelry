<!DOCTYPE html>
<html lang="sq">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>ALLOYEDGE Jewelry</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&family=Playfair+Display:wght@600;700&display=swap" rel="stylesheet">

<style>

body{
    margin:0;
    font-family:'Poppins', sans-serif;
    background: linear-gradient(135deg, #ffe6f0, #e8f5e9);
    overflow-x:hidden;
}

/* Gjethe dekorative */
body::before{
    content:"";
    position:fixed;
    width:100%;
    height:100%;
    background-image:url('logo.png');
    background-repeat:no-repeat;
    background-position:center;
    background-size:600px;
    opacity:0.05;
    z-index:-1;
}

header{
    display:flex;
    justify-content:space-between;
    align-items:center;
    padding:20px 8%;
    background:rgba(255,255,255,0.7);
    backdrop-filter:blur(10px);
    position:fixed;
    width:100%;
}

header img{
    height:55px;
}

nav a{
    text-decoration:none;
    margin-left:30px;
    color:#b76e79;
    font-weight:500;
    transition:0.3s;
}

nav a:hover{
    color:#2e7d32;
}

.hero{
    height:100vh;
    display:flex;
    align-items:center;
    justify-content:center;
    text-align:center;
    padding:0 20px;
}

.hero h1{
    font-family:'Playfair Display', serif;
    font-size:56px;
    background: linear-gradient(to right, #b76e79, #2e7d32);
    -webkit-background-clip:text;
    -webkit-text-fill-color:transparent;
}

.hero p{
    font-size:20px;
    margin:20px 0;
    color:#555;
}

.btn{
    padding:14px 35px;
    border-radius:40px;
    border:none;
    font-size:16px;
    cursor:pointer;
    background:linear-gradient(to right, #b76e79, #2e7d32);
    color:white;
    transition:0.4s;
}

.btn:hover{
    transform:scale(1.05);
    box-shadow:0 10px 25px rgba(0,0,0,0.2);
}

.section{
    padding:100px 10%;
    text-align:center;
}

.section h2{
    font-family:'Playfair Display', serif;
    font-size:40px;
    color:#b76e79;
}

.products{
    display:grid;
    grid-template-columns:repeat(auto-fit, minmax(250px,1fr));
    gap:40px;
    margin-top:50px;
}

.card{
    background:white;
    padding:25px;
    border-radius:25px;
    box-shadow:0 15px 35px rgba(0,0,0,0.1);
    transition:0.4s;
}

.card:hover{
    transform:translateY(-10px);
}

.card img{
    width:100%;
    border-radius:20px;
}

.card h3{
    color:#2e7d32;
}

footer{
    background:linear-gradient(to right, #b76e79, #2e7d32);
    color:white;
    padding:40px;
    text-align:center;
}

@media(max-width:768px){
    .hero h1{
        font-size:36px;
    }
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
    <div>
        <h1>Shkëlqe çdo ditë ✨</h1>
        <p>Bizhuteri elegante dhe moderne për vajza që duan stil, feminitet dhe vetëbesim.</p>
        <button class="btn">Shiko Koleksionin</button>
    </div>
</section>

<section class="section" id="produkte">
    <h2>Koleksioni Ynë</h2>
    <div class="products">
        <div class="card">
            <img src="https://via.placeholder.com/300x300">
            <h3>Vathë Elegant</h3>
            <p>19.99€</p>
        </div>
        <div class="card">
            <img src="https://via.placeholder.com/300x300">
            <h3>Qafore Delikate</h3>
            <p>24.99€</p>
        </div>
        <div class="card">
            <img src="https://via.placeholder.com/300x300">
            <h3>Unazë Minimaliste</h3>
            <p>17.99€</p>
        </div>
    </div>
</section>

<section class="section" id="rreth">
    <h2>Rreth ALLOYEDGE</h2>
    <p>ALLOYEDGE është një dyqan online bizhuterish për vajza të reja që duan të ndihen elegante dhe të sigurta. Çdo model është i përzgjedhur me kujdes për të sjellë stil modern dhe finesë.</p>
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
