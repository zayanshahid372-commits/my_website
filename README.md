!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Mujia Farmhouse</title>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: Arial, sans-serif;
}

html {
  scroll-behavior: smooth;
}

body {
  background: #fff;
  color: #222;
}

header {
  background: #123d2a;
  color: white;
  padding: 20px 8%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
}

.logo {
  font-size: 26px;
  font-weight: bold;
  color: #e5c77a;
}

nav a {
  color: white;
  text-decoration: none;
  margin-left: 20px;
}

.hero {
  height: 600px;
  background:
    linear-gradient(#0006,#0007),
    url('https://images.unsplash.com/photo-1449158743715-0a90ebb6d2d8')
    center/cover;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  color: white;
  padding: 20px;
}

.hero h1 {
  font-size: 55px;
  margin-bottom: 15px;
}

.hero p {
  font-size: 20px;
  margin-bottom: 25px;
}

.btn {
  display: inline-block;
  background: #d5b45b;
  color: #123d2a;
  padding: 14px 28px;
  border-radius: 5px;
  text-decoration: none;
  font-weight: bold;
}

section {
  padding: 65px 8%;
  text-align: center;
}

h2 {
  color: #174b32;
  font-size: 34px;
  margin-bottom: 25px;
}

.about p {
  max-width: 750px;
  margin: auto;
  line-height: 1.8;
}

.facilities {
  background: #f4f6f0;
}

.cards {
  display: grid;
  grid-template-columns: repeat(auto-fit,minmax(220px,1fr));
  gap: 22px;
}

.card {
  background: white;
  padding: 30px 20px;
  border-radius: 12px;
  box-shadow: 0 3px 15px #0001;
}

.card h3 {
  color: #174b32;
  margin: 15px 0;
}

.gallery-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit,minmax(230px,1fr));
  gap: 15px;
}

.gallery-grid img {
  width: 100%;
  height: 220px;
  object-fit: cover;
  border-radius: 10px;
}

.booking {
  background: #f4f6f0;
}

form {
  max-width: 500px;
  margin: auto;
}

input, select, textarea {
  width: 100%;
  padding: 14px;
  margin: 9px 0;
  border: 1px solid #ccc;
  border-radius: 5px;
}

button {
  background: #174b32;
  color: white;
  padding: 15px;
  border: none;
  width: 100%;
  cursor: pointer;
  border-radius: 5px;
  font-size: 16px;
}

footer {
  background: #123d2a;
  color: white;
  text-align: center;
  padding: 30px;
}

@media(max-width:600px) {
  header {
    justify-content: center;
    gap: 15px;
  }
  nav a {
    margin: 7px;
    display: inline-block;
  }
  .hero h1 {
    font-size: 38px;
  }
}
</style>
</head>

<body>

<header>
  <div class="logo">Mujia Farmhouse</div>
  <nav>
    <a href="#home">Home</a>
    <a href="#about">About</a>
    <a href="#facilities">Facilities</a>
    <a href="#gallery">Gallery</a>
    <a href="#booking">Booking</a>
  </nav>
</header>

<div class="hero" id="home">
  <div>
    <h1>Welcome to Mujia Farmhouse</h1>
    <p>Enjoy Nature, Luxury & Beautiful Moments</p>
    <a href="#booking" class="btn">Book Your Stay</a>
  </div>
</div>

<section class="about" id="about">
  <h2>About Our Farmhouse</h2>
  <p>
    Welcome to Mujia Farmhouse! Enjoy a peaceful environment,
    beautiful greenery and unforgettable moments with your
    family and friends. Your perfect destination for relaxation
    and celebrations.
  </p>
</section>

<section class="facilities" id="facilities">
  <h2>Our Facilities</h2>
  <div class="cards">
    <div class="card">
      <h3>🏊 Swimming Pool</h3>
      <p>Enjoy refreshing swimming time.</p>
    </div>
    <div class="card">
      <h3>🌳 Green Garden</h3>
      <p>Beautiful green surroundings.</p>
    </div>
    <div class="card">
      <h3>🎉 Party Area</h3>
      <p>Perfect for family events and parties.</p>
    </div>
    <div class="card">
      <h3>🍖 BBQ Area</h3>
      <p>Enjoy BBQ with friends and family.</p>
    </div>
  </div>
</section>

<section id="gallery">
  <h2>Our Gallery</h2>
  <div class="gallery-grid">
    <img src="https://images.unsplash.com/photo-1449158743715-0a90ebb6d2d8" alt="Farmhouse">
    <img src="https://images.unsplash.com/photo-1600585154340-be6161a56a0c" alt="House">
    <img src="https://images.unsplash.com/photo-1576013551627-0cc20b96c2a7" alt="Swimming pool">
    <img src="https://images.unsplash.com/photo-1470770841072-f978cf4d019e" alt="Nature">
  </div>
</section>

<section class="booking" id="booking">
  <h2>Book Your Farmhouse</h2>
  <form onsubmit="bookNow(event)">
    <input id="name" type="text" placeholder="Your Name" required>
    <input id="phone" type="tel" placeholder="Phone Number" required>
    <input id="date" type="date" required>
    <select id="guests" required>
      <option value="">Number of Guests</option>
      <option>1-10</option>
      <option>10-20</option>
      <option>20-50</option>
      <option>50+</option>
    </select>
    <textarea id="message" placeholder="Your Message"></textarea>
    <button type="submit">Book on WhatsApp</button>
  </form>
</section>

<footer>
  <h3>Mujia Farmhouse</h3>
  <p>Enjoy Life, Nature & Happiness</p>
  <p>© 2026 Mujia Farmhouse. All Rights Reserved.</p>
</footer>

<script>
function bookNow(event) {
  event.preventDefault();

  const name = document.getElementById('name').value;
  const phone = document.getElementById('phone').value;
  const date = document.getElementById('date').value;
  const guests = document.getElementById('guests').value;
  const message = document.getElementById('message').value;

  // Apna WhatsApp number country code ke sath likhein
  const whatsappNumber = "923001234567";

  const text = `Farmhouse Booking Request
Name: ${name}
Phone: ${phone}
Date: ${date}
Guests: ${guests}
Message: ${message}`;

  window.open(
    `https://wa.me/${whatsappNumber}?text=${encodeURIComponent(text)}`,
    '_blank'
  );
}
</script>

</body>
</html>
