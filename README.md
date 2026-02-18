<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>ALLOYEDGE Jewelry</title>

<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;600&family=Montserrat:wght@300;400;500&display=swap" rel="stylesheet">

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    scroll-behavior:smooth;
}

body{
    font-family:'Montserrat', sans-serif;
    background:#0f2e24;
    color:white;
}

/* NAVIGATION */
nav{
    position:fixed;
    width:100%;
    padding:20px 60px;
    display:flex;
    justify-content:space-between;
    align-items:center;
    background:rgba(15,46,36,0.8);
    backdrop-filter:blur(10px);
    z-index:1000;
}

nav h2{
    font-family:'Playfair Display', serif;
    letter-spacing:5px;
}

nav a{
    color:white;
    text-decoration:none;
    margin-left:30px;
    font-size:14px;
    letter-spacing:2px;
    transition:0.3s;
}

nav a:hover{
    color:#f5c6dc;
}

/* HERO */
.hero{
    height:100vh;
    display:flex;
    flex-direction:column;
    justify-content:center;
    align-items:center;
    text-align:center;
    padding:20px;
    background:linear-gradient(135deg,#f3c5da,#0f2e24);
}

.hero h1{
    font-family:'Playfair Display', serif;
    font-size:70px;
    letter-spacing:10px;
}

.hero p{
    margin-top:20px;
    font-size:18px;
    letter-spacing:3px;
}

.button{
    margin-top:50px;
    padding:15px 45px;
    border:1px solid white;
    background:transparent;
    color:white;
    letter-spacing:3px;
    cursor:pointer;
    transition:0.4s;
}

.button:hover{
    background:white;
    color:#0f2e24;
}

/* SECTIONS */
section{
    padding:120px 60px;
    text-align:center;
}

.section-title{
    font-family:'Playfair Display', serif;
    font-size:40px;
    margin-bottom:40px;
    letter-spacing:5px;
}

/* ABOUT */
.about{
    background:#0f2e24;
    max-width:800px;
    margin:auto;
    font-size:18px;
    line-height:1.8;
    opacity:0.9;
}

/* COLLECTION */
.collection{
    background:#f3c5da;
    color:#0f2e24;
}

.collection p{
    max-width:700px;
    margin:auto;
    font-size:18px;
    line-height:1.8;
}

/* ORDER */
.order{
    background:#0f2e24;
}

/* POPUP */
.popup{
    position:fixed;
    top:50%;
    left:50%;
    transform:translate(-50%,-50%);
    background:#111;
    padding:50px;
    border-radius:10px;
    text-align:center;
    display:none;
    z-index:2000;
}

.popup h3{
    margin-bottom:20px;
}

.popup a{
    display:block;
    color:#f3c5da;
    font-size:18px;
    margin:15px 0;
    text-decoration:none;
    transition:0.3s;
}

.popup a:hover{
    color:white;
}

.close{
    position:absolute;
    top:10px;
    right:20px;
    cursor:pointer;
    font-size:22px;
}

footer{
    padding:30px;
    text-align:center;
    background:#0a1f18;
    font-size:12px;
    letter-spacing:2px;
}
</style>
</head>

<body>

<nav>
<h2>ALLOYEDGE</h2>
<div>
<a href="#about">ABOUT</a>
<a href="#collection">COLLECTION</a>
<a href="#order">ORDER</a>
</div>
</nav>

<section class="hero">
<h1>ALLOYEDGE</h1>
<p>FEMININE JEWELRY COLLECTION</p>
<button class="button" onclick="openPopup()">ORDER NOW</button>
</section>

<section id="about">
<div class="section-title">ABOUT</div>
<div class="about">
ALLOYEDGE is a curated feminine jewelry selection designed to elevate your everyday elegance.  
Each piece is chosen to express softness, confidence, and luxury — made for women who love refined beauty.
</div>
</section>

<section id="collection" class="collection">
<div class="section-title">COLLECTION</div>
<p>
Discover timeless necklaces, delicate bracelets, elegant rings, and statement earrings.  
Crafted to complement every occasion — from everyday sophistication to special moments.
</p>
</section>

<section id="order" class="order">
<div class="section-title">ORDER NOW</div>
<button class="button" onclick="openPopup()">CONTACT US</button>
</section>

<div class="popup" id="popup">
<div class="close" onclick="closePopup()">×</div>
<h3>Order via</h3>
<a href="https://www.instagram.com/alloyedge.jewelry" target="_blank">
Instagram @alloyedge.jewelry
</a>
<a href="https://www.tiktok.com/@alloyedge.jewelry" target="_blank">
TikTok @alloyedge.jewelry
</a>
</div>

<footer>
© 2026 ALLOYEDGE Jewelry
</footer>

<script>
function openPopup(){
    document.getElementById("popup").style.display="block";
}
function closePopup(){
    document.getElementById("popup").style.display="none";
}
</script>

</body>
</html>
