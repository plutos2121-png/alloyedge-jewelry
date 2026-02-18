<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>ALLOYEDGE Jewelry</title>

<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@500;700&family=Montserrat:wght@300;400&display=swap" rel="stylesheet">

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

body{
    font-family:'Montserrat', sans-serif;
    background:linear-gradient(160deg,#f4c6dc,#0e2f24);
    color:white;
    display:flex;
    justify-content:center;
    align-items:center;
    height:100vh;
    text-align:center;
}

/* MAIN CONTAINER */
.container{
    width:90%;
    max-width:400px;
}

/* TITLE */
h1{
    font-family:'Playfair Display', serif;
    font-size:42px;
    letter-spacing:8px;
}

.subtitle{
    margin-top:15px;
    font-size:14px;
    letter-spacing:3px;
    opacity:0.85;
}

/* BUTTON */
.order-btn{
    margin-top:50px;
    padding:15px;
    width:100%;
    border:1px solid white;
    background:transparent;
    color:white;
    letter-spacing:3px;
    font-size:14px;
    cursor:pointer;
    transition:0.4s;
}

.order-btn:hover{
    background:white;
    color:#0e2f24;
}

/* POPUP */
.popup{
    position:fixed;
    bottom:0;
    left:0;
    width:100%;
    background:#111;
    padding:40px 20px;
    border-top-left-radius:20px;
    border-top-right-radius:20px;
    display:none;
}

.popup h3{
    margin-bottom:25px;
    letter-spacing:3px;
}

.popup a{
    display:block;
    color:#f4c6dc;
    font-size:16px;
    margin:15px 0;
    text-decoration:none;
}

.popup a:hover{
    color:white;
}

.close{
    position:absolute;
    top:15px;
    right:25px;
    font-size:20px;
    cursor:pointer;
}
</style>
</head>

<body>

<div class="container">
    <h1>ALLOYEDGE</h1>
    <div class="subtitle">FEMININE JEWELRY</div>

    <button class="order-btn" onclick="openPopup()">ORDER NOW</button>
</div>

<div class="popup" id="popup">
    <div class="close" onclick="closePopup()">✕</div>
    <h3>ORDER VIA</h3>

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
    document.getElementById("popup").style.display="block";
    document.getElementById("popup").style.animation="slideUp 0.4s ease";
}

function closePopup(){
    document.getElementById("popup").style.display="none";
}
</script>

</body>
</html>
