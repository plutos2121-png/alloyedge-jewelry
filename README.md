<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>ALLOYEDGE Jewelry</title>

<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;600&family=Montserrat:wght@300;400&display=swap" rel="stylesheet">

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

body{
    font-family:'Montserrat', sans-serif;
    background: linear-gradient(135deg,#f5d6e6,#1f4d3a);
    color:white;
    overflow-x:hidden;
}

.hero{
    height:100vh;
    display:flex;
    flex-direction:column;
    justify-content:center;
    align-items:center;
    text-align:center;
    padding:20px;
}

.logo{
    width:280px;
    margin-bottom:30px;
}

h1{
    font-family:'Playfair Display', serif;
    font-size:60px;
    letter-spacing:8px;
    font-weight:600;
}

.tagline{
    margin-top:20px;
    font-size:18px;
    letter-spacing:3px;
    opacity:0.9;
}

.button{
    margin-top:50px;
    padding:15px 40px;
    border:1px solid white;
    background:transparent;
    color:white;
    font-size:16px;
    letter-spacing:3px;
    cursor:pointer;
    transition:0.4s ease;
}

.button:hover{
    background:white;
    color:#1f4d3a;
}

.popup{
    position:fixed;
    top:50%;
    left:50%;
    transform:translate(-50%,-50%);
    background:rgba(0,0,0,0.85);
    padding:40px;
    border-radius:10px;
    text-align:center;
    display:none;
}

.popup a{
    display:block;
    color:#f5d6e6;
    font-size:20px;
    margin:20px 0;
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
    font-size:25px;
    cursor:pointer;
}

footer{
    position:absolute;
    bottom:20px;
    width:100%;
    text-align:center;
    font-size:12px;
    opacity:0.7;
    letter-spacing:2px;
}
</style>
</head>

<body>

<section class="hero">

<h1>ALLOYEDGE</h1>
<div class="tagline">FEMININE JEWELRY COLLECTION</div>

<button class="button" onclick="openPopup()">ORDER NOW</button>

<footer>
© 2026 ALLOYEDGE Jewelry
</footer>

</section>

<div class="popup" id="popup">
<div class="close" onclick="closePopup()">×</div>
<h2>Order via</h2>
<a href="https://www.instagram.com/alloyedge.jewelry" target="_blank">
Instagram @alloyedge.jewelry
</a>
<a href="https://www.tiktok.com/@alloyedge.jewelry" target="_blank">
TikTok @alloyedge.jewelry
</a>
</div>

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
