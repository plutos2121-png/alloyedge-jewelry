<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>ALLOYEDGE® | Luxury Jewelry</title>

<style>
body {
    margin: 0;
    font-family: 'Arial', sans-serif;
    background: linear-gradient(to bottom, #f8e8ec, #ffffff);
    color: #333;
}

header {
    background: url("hero.jpg") no-repeat center center/cover;
    text-align: center;
    padding: 140px 20px;
    color: white;
}

header h1 {
    font-size: 60px;
    margin: 0;
    letter-spacing: 5px;
}

header p {
    font-size: 20px;
    margin-top: 15px;
}

section {
    padding: 60px 20px;
    text-align: center;
}

.button {
    background-color: #caa24c;
    color: white;
    padding: 15px 30px;
    text-decoration: none;
    border-radius: 30px;
    font-weight: bold;
    display: inline-block;
    margin-top: 20px;
    transition: 0.3s;
}

.button:hover {
    background-color: #b89035;
}

.products {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 30px;
}

.product-card {
    background: white;
    padding: 25px;
    width: 250px;
    border-radius: 15px;
    box-shadow: 0 10px 25px rgba(0,0,0,0.1);
}

.product-card h3 {
    color: #caa24c;
}

footer {
    background: #1f3d2b;
    color: white;
    text-align: center;
    padding: 20px;
}
</style>

<script>
function openSocials() {
    window.open("https://www.tiktok.com/@alloyedge.jewelry", "_blank");
    window.open("https://instagram.com/alloyedge.jewelry", "_blank");
}
</script>

</head>

<body>

<header>
    <h1>ALLOYEDGE®</h1>
    <p>Curated Elegance for Modern Women</p>
    <a href="#shop" class="button">Explore Collection</a>
</header>

<section id="about">
    <h2>About Us</h2>
    <p>
    ALLOYEDGE® Jewelry is a curated boutique offering feminine and elegant jewelry pieces 
    selected for women who appreciate beauty and modern style.
    Each piece is carefully chosen to elevate your everyday look.
    </p>
</section>

<section id="shop">
    <h2>Our Collection</h2>
    <div class="products">

        <div class="product-card">
            <h3>Golden Necklace</h3>
            <p>Soft luxury with modern touch.</p>
        </div>

        <div class="product-card">
            <h3>Silver Necklace</h3>
            <p>Minimal elegance with timeless shine.</p>
        </div>

    </div>
</section>

<section>
    <h2>How To Order</h2>
    <p>
    Orders are placed via Instagram or TikTok message.  
    Payment is made upon delivery (Cash on Delivery).
    </p>

    <a href="javascript:void(0);" onclick="openSocials()" class="button">
        Order Now
    </a>
</section>

<footer>
    © 2026 ALLOYEDGE® – All Rights Reserved
</footer>

</body>
</html>
