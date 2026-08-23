<!DOCTYPE html>
<html lang="bn">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Followers Master</title>

  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: Arial, sans-serif;
    }

    body {
      background: #0b0b12;
      color: white;
    }

    header {
      padding: 20px;
      text-align: center;
      background: linear-gradient(135deg,#833ab4,#fd1d1d,#fcb045);
    }

    header h1 {
      font-size: 30px;
    }

    header p {
      margin-top: 6px;
    }

    .hero {
      text-align: center;
      padding: 55px 20px;
    }

    .hero h2 {
      font-size: 35px;
      margin-bottom: 12px;
    }

    .hero p {
      color: #bbb;
      margin-bottom: 25px;
    }

    .btn {
      display: inline-block;
      padding: 13px 25px;
      border-radius: 30px;
      background: #ff3b81;
      color: white;
      text-decoration: none;
      font-weight: bold;
    }

    .services {
      padding: 25px;
      max-width: 1000px;
      margin: auto;
    }

    .services h2 {
      text-align: center;
      margin-bottom: 25px;
    }

    .cards {
      display: grid;
      grid-template-columns: repeat(auto-fit,minmax(220px,1fr));
      gap: 18px;
    }

    .card {
      background: #171722;
      padding: 25px;
      border-radius: 18px;
      text-align: center;
      border: 1px solid #29293a;
    }

    .card h3 {
      margin-bottom: 10px;
    }

    .price {
      font-size: 24px;
      color: #ff4d91;
      margin: 15px 0;
      font-weight: bold;
    }

    .order {
      padding: 35px 20px;
      max-width: 600px;
      margin: auto;
      text-align: center;
    }

    input, select {
      width: 100%;
      padding: 14px;
      margin: 8px 0;
      border: none;
      border-radius: 10px;
      background: #1b1b27;
      color: white;
    }

    button {
      width: 100%;
      padding: 14px;
      margin-top: 12px;
      border: none;
      border-radius: 10px;
      background: #ff3b81;
      color: white;
      font-size: 16px;
      font-weight: bold;
    }

    footer {
      text-align: center;
      padding: 25px;
      color: #aaa;
      background: #08080d;
      margin-top: 30px;
    }
  </style>
</head>

<body>

<header>
  <h1>Followers Master</h1>
  <p>Social Media Growth & Creative Services</p>
</header>

<section class="hero">
  <h2>Grow Your Social Presence 🚀</h2>
  <p>Professional social-media marketing and creative services.</p>
  <a href="#order" class="btn">Get Started</a>
</section>

<section class="services">
  <h2>Our Services</h2>

  <div class="cards">

    <div class="card">
      <h3>📱 Instagram Marketing</h3>
      <p>Promotional and creative marketing support.</p>
      <div class="price">From ₹20</div>
      <a href="#order" class="btn">Order</a>
    </div>

    <div class="card">
      <h3>❤️ Content Promotion</h3>
      <p>Help promote your social-media content.</p>
      <div class="price">From ₹20</div>
      <a href="#order" class="btn">Order</a>
    </div>

    <div class="card">
      <h3>▶️ Video Promotion</h3>
      <p>Creative promotion for your videos.</p>
      <div class="price">From ₹20</div>
      <a href="#order" class="btn">Order</a>
    </div>

  </div>
</section>

<section class="order" id="order">
  <h2>Place Your Request</h2>

  <input type="text" id="name" placeholder="Your Name">

  <input type="text" id="username"
         placeholder="Instagram Username">

  <select id="service">
    <option>Instagram Marketing</option>
    <option>Content Promotion</option>
    <option>Video Promotion</option>
  </select>

  <button onclick="sendOrder()">Submit Request</button>
</section>

<footer>
  © 2026 Followers Master — All Rights Reserved
</footer>

<script>
function sendOrder() {

  let name = document.getElementById("name").value;
  let username = document.getElementById("username").value;
  let service = document.getElementById("service").value;

  if(name === "" || username === "") {
    alert("Please fill all details.");
    return;
  }

  alert(
    "Request submitted!\\n\\n" +
    "Name: " + name +
    "\\nUsername: " + username +
    "\\nService: " + service
  );
}
</script>

</body>
</html>
