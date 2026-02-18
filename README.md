<!DOCTYPE html>
<html lang="sq">
<head>
  <meta charset="UTF-8">
  <title>AlloyEdge | Jewelry for Women</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>

  <header>
    <h1>AlloyEdge</h1>
    <p>Elegancë që shkëlqen ✨</p>
    <nav>
      <a href="#about">Rreth Nesh</a>
      <a href="#products">Produktet</a>
      <a href="#contact">Kontakt</a>
    </nav>
  </header>

  <section id="hero">
    <h2>Zbulo Koleksionin Tonë</h2>
    <button onclick="scrollToProducts()">Shiko Produktet</button>
  </section>

  <section id="products">
    <h2>Koleksioni</h2>
    <div class="product-container">
      <div class="product">
        <img src="https://via.placeholder.com/250" alt="Varëse">
        <h3>Varëse Elegant</h3>
        <p>€25</p>
      </div>

      <div class="product">
        <img src="https://via.placeholder.com/250" alt="Vathë">
        <h3>Vathë Modern</h3>
        <p>€18</p>
      </div>

      <div class="product">
        <img src="https://via.placeholder.com/250" alt="Byzylyk">
        <h3>Byzylyk Luksoz</h3>
        <p>€30</p>
      </div>
    </div>
  </section>

  <section id="about">
    <h2>Rreth AlloyEdge</h2>
    <p>AlloyEdge ofron bizhuteri elegante dhe moderne për femra që duan të shkëlqejnë çdo ditë.</p>
  </section>

  <section id="contact">
    <h2>Na Kontakto</h2>
    <p>Email: info@alloyedge.com</p>
    <p>Instagram: @alloyedge</p>
  </section>

  <footer>
    <p>© 2026 AlloyEdge. Të gjitha të drejtat e rezervuara.</p>
  </footer>

  <script src="script.js"></script>
</body>
</html>
body {
  margin: 0;
  font-family: Arial, sans-serif;
  background-color: #f9f6f2;
  color: #333;
  text-align: center;
}

header {
  background-color: #000;
  color: white;
  padding: 20px;
}

nav a {
  color: white;
  margin: 0 15px;
  text-decoration: none;
}

#hero {
  padding: 60px;
  background: linear-gradient(to right, #d4af37, #f5e6c4);
}

button {
  padding: 10px 20px;
  border: none;
  background-color: black;
  color: white;
  cursor: pointer;
}

.product-container {
  display: flex;
  justify-content: center;
  gap: 20px;
  padding: 40px;
  flex-wrap: wrap;
}

.product {
  background: white;
  padding: 15px;
  border-radius: 10px;
  box-shadow: 0 5px 15px rgba(0,0,0,0.1);
}
function scrollToProducts() {
  document.getElementById("products").scrollIntoView({ 
    behavior: "smooth" 
  });
}
