
<html lang="sq">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>ALLOYEDGE | Jewelry for Women</title>

<style>
body {
  margin: 0;
  font-family: 'Segoe UI', sans-serif;
  background: linear-gradient(to bottom, #ffe6f2, #ffffff);
  color: #444;
  text-align: center;
}

/* HEADER */
header {
  background: #ff4da6;
  color: white;
  padding: 30px 20px;
}

header h1 {
  margin: 0;
  font-size: 40px;
  letter-spacing: 4px;
}

header p {
  margin-top: 5px;
  font-style: italic;
}

nav a {
  color: white;
  margin: 0 15px;
  text-decoration: none;
  font-weight: bold;
}

/* HERO */
#hero {
  padding: 80px 20px;
  background: #ffd6eb;
}

#hero h2 {
  font-size: 28px;
  color: #ff1a8c;
}

button {
  padding: 12px 30px;
  border: none;
  background: #ff1a8c;
  color: white;
  cursor: pointer;
  border-radius: 25px;
  font-size: 16px;
  margin-top: 20px;
}

button:hover {
  background: #cc0066;
}

/* PRODUCTS */
.products {
  display: flex;
  justify-content: center;
  gap: 25px;
  flex-wrap: wrap;
  padding: 50px 20px;
}

.product {
  background: white;
  padding: 20px;
  border-radius: 15px;
  width: 250px;
  box-shadow: 0 10px 25px rgba(255, 105, 180, 0.2);
  transition: transform 0.3s ease;
}

.product:hover {
  transform: scale(1.05);
}

.product img {
  width: 100%;
  border-radius: 12px;
}

/* SECTIONS */
section h2 {
  color: #ff1a8c;
  margin-top: 40px;
}

/* FOOTER */
footer {
  background: #ff4da6;
  color: white;
  padding: 20px;
  margin-top: 40px;
}
</style>

</head>
<body>

<header>
  <h1>ALLOYEDGE</h1>
  <p>Elegancë • Stil • Shkëlqim</p>
  <nav>
    <a href="#products">Produktet</a>
    <a href="#about">Rreth Nesh</a>
    <a href="#contact">Kontakt</a>
  </nav>
</header>

<section id="hero">
  <h2>Zbulo Koleksionin Tonë Ekskluziv</h2>
  <button onclick="document.getElementById('products').scrollIntoView({behavior:'smooth'})">
    Shiko Tani
  </button>
</section>

<section id="products">
  <h2>Koleksioni</h2>
  <div class="products">

    <div class="product">
      <img src="https://via.placeholder.com/250" alt="Varëse">
      <h3>Varëse Rozë</h3>
      <p>€25</p>
    </div>

    <div class="product">
      <img src="https://via.placeholder.com/250" alt="Vathë">
      <h3>Vathë Elegant</h3>
      <p>€18</p>
    </div>

    <div class="product">
      <img src="https://via.placeholder.com/250" alt="Byzylyk">
      <h3>Byzylyk Glam</h3>
      <p>€30</p>
    </div>

  </div>
</section>

<section id="about">
  <h2>Rreth Nesh</h2>
  <p>ALLOYEDGE krijon bizhuteri për femra që duan të ndihen të bukura, elegante dhe unike çdo ditë.</p>
</section>

<section id="contact">
  <h2>Na Kontakto</h2>
  <p>tik tok: @alloyedge.jewelry</p>
  <p>Instagram: @alloyedge.jewelry</p>
</section>

<footer>
  <p>© 2026 ALLOYEDGE. Të gjitha të drejtat e rezervuara.</p>
</footer>

</body>
</html>
