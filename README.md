<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Luxury Watches & Jewelry | Demo</title>

  <style>
    body {
      margin: 0;
      font-family: "Helvetica Neue", Arial, sans-serif;
      background: #0b0b0b;
      color: #ffffff;
    }

    header {
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 20px 40px;
      border-bottom: 1px solid #222;
      background: #000;
    }

    header img {
      height: 40px;
    }

    nav a {
      color: #b0b0b0;
      text-decoration: none;
      margin-left: 20px;
      font-size: 14px;
    }

    nav a:hover {
      color: #ffffff;
    }

    /* Hero Banner Rotation */
    .hero {
      position: relative;
      height: 80vh;
      overflow: hidden;
    }

    .slides {
      height: 100%;
      width: 100%;
      position: relative;
    }

    .slide {
      position: absolute;
      inset: 0;
      background-size: cover;
      background-position: center;
      opacity: 0;
      transition: opacity 1.5s ease-in-out;
    }

    .slide.active {
      opacity: 1;
    }

    .hero-overlay {
      position: absolute;
      inset: 0;
      background: linear-gradient(to right, rgba(0,0,0,0.7), rgba(0,0,0,0.2));
      display: flex;
      align-items: center;
      padding-left: 80px;
    }

    .hero-content h1 {
      font-size: 48px;
      font-weight: 300;
      margin-bottom: 20px;
    }

    .hero-content button {
      padding: 14px 30px;
      border: none;
      background: #ffffff;
      color: #000;
      font-size: 12px;
      letter-spacing: 1px;
      cursor: pointer;
      border-radius: 30px;
    }

    section {
      padding: 80px 40px;
      text-align: center;
    }

    .agent-demo {
      max-width: 700px;
      margin: auto;
      border: 2px dashed #c9a24d;
      padding: 40px;
      margin-top: 30px;
      border-radius: 6px;
      color: #c9a24d;
      font-size: 14px;
    }

    footer {
      padding: 40px;
      text-align: center;
      border-top: 1px solid #222;
      color: #888;
    }

    @media (max-width: 768px) {
      nav {
        display: none;
      }

      .hero-overlay {
        padding-left: 30px;
      }

      .hero-content h1 {
        font-size: 32px;
      }
    }
  </style>
</head>

<body>

  <!-- Header -->
  <header>
    <img src="logo.png" alt="Brand Logo" />
    <nav>
      <a href="#">Watches</a>
      <a href="#">Jewelry</a>
      <a href="#">Pre-Owned</a>
      <a href="#">Sell & Trade</a>
      <a href="#">Contact</a>
    </nav>
  </header>

  <!-- Hero with Rotating Banners -->
  <div class="hero">
    <div class="slides">
      <div class="slide active" style="background-image: url('banner.png')"></div>
      <div class="slide" style="background-image: url('banner1.png')"></div>
      <div class="slide" style="background-image: url('banner2.png')"></div>
      <div class="slide" style="background-image: url('banner3.png')"></div>
      <div class="slide" style="background-image: url('banner4.png')"></div>
    </div>

    <div class="hero-overlay">
      <div class="hero-content">
        <h1>Timeless Icons of Luxury</h1>
        <button>EXPLORE COLLECTION</button>
      </div>
    </div>
  </div>

  <!-- Agentforce Demo Section -->
  <section>
    <h2>Ask Our Watch Advisor</h2>
    <p>
      AI-powered guidance for collectors and partners — grounded in trusted
      product and authentication knowledge.
    </p>

    <div class="agent-demo">
      🤖 Agentforce Web Agent Demo Area<br><br>
      • Salesforce Knowledge grounded answers<br>
      • B2C & B2B ready<br>
      • Smart escalation to sales or service
    </div>
  </section>

  <!-- Footer -->
  <footer>
    © 2026 Demo Luxury Company. All rights reserved.
  </footer>

  <!-- Banner Rotation Script -->
  <script>
    const slides = document.querySelectorAll(".slide");
    let currentSlide = 0;

    setInterval(() => {
      slides[currentSlide].classList.remove("active");
      currentSlide = (currentSlide + 1) % slides.length;
      slides[currentSlide].classList.add("active");
    }, 5000);
  </script>

</body>
</html>
