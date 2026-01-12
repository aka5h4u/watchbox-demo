<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Luxury Watches & Jewelry | Demo</title>

  <style>
    :root {
      --black: #0b0b0b;
      --gold: #c9a24d;
      --muted: #b0b0b0;
    }

    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      font-family: "Helvetica Neue", Arial, sans-serif;
      background: var(--black);
      color: #fff;
    }

    /* Header */
    header {
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 20px 40px;
      border-bottom: 1px solid #1f1f1f;
      background: #000;
    }

    .logo img {
      height: 40px;
    }

    nav a {
      color: var(--muted);
      text-decoration: none;
      margin-left: 24px;
      font-size: 0.95rem;
    }

    nav a:hover {
      color: var(--gold);
    }

    /* Hero Slider */
    .hero {
      position: relative;
      height: 85vh;
      overflow: hidden;
    }

    .slides {
      display: flex;
      height: 100%;
      width: 500%;
      animation: slide 30s infinite;
    }

    .slide {
      width: 100%;
      flex-shrink: 0;
      background-size: cover;
      background-position: center;
    }

    .overlay {
      position: absolute;
      inset: 0;
      background: linear-gradient(to right, rgba(0,0,0,0.75), rgba(0,0,0,0.2));
      display: flex;
      align-items: center;
      padding-left: 80px;
    }

    .overlay-content h1 {
      font-size: 3rem;
      font-weight: 300;
      margin-bottom: 20px;
    }

    .overlay-content button {
      background: #fff;
      border: none;
      padding: 14px 28px;
      font-size: 0.9rem;
      letter-spacing: 1px;
      cursor: pointer;
      border-radius: 30px;
    }

    /* Slider animation */
    @keyframes slide {
      0% { transform: translateX(0); }
      20% { transform: translateX(0); }
      25% { transform: translateX(-100%); }
      40% { transform: translateX(-100%); }
      45% { transform: translateX(-200%); }
      60% { transform: translateX(-200%); }
      65% { transform: translateX(-300%); }
      80% { transform: translateX(-300%); }
      85% { transform: translateX(-400%); }
      100% { transform: translateX(-400%); }
    }

    /* AI Section */
    section {
      padding: 80px 40px;
      text-align: center;
    }

    .agent-box {
      max-width: 700px;
      margin: auto;
      border: 2px dashed var(--gold);
      padding: 40px;
      margin-top: 30px;
      border-radius: 6px;
      font-size: 0.95rem;
    }

    footer {
      padding: 40px;
      text-align: center;
      color: var(--muted);
      border-top: 1px solid #1f1f1f;
    }

    @media (max-width: 768px) {
      nav {
        display: none;
      }

      .overlay {
        padding-left: 30px;
      }

      .overlay-content h1 {
        font-size: 2rem;
      }
    }
  </style>
</head>

<body>

  <!-- Header -->
  <header>
    <div class="logo">
      <img src="/watchbox-demo/images/logo.png" alt="Logo">
    </div>
    <nav>
      <a href="#">Watches</a>
      <a href="#">Jewelry</a>
      <a href="#">Pre-Owned</a>
      <a href="#">Sell & Trade</a>
      <a href="#">Contact</a>
    </nav>
  </header>

  <!-- Hero Slider -->
  <div class="hero">
    <div class="slides">
      <div class="slide" style="background-image:url('./images/banner.png')"></div>
      <div class="slide" style="background-image:url('./images/banner1.png')"></div>
      <div class="slide" style="background-image:url('./images/banner2.png')"></div>
      <div class="slide" style="background-image:url('./images/banner3.png')"></div>
      <div class="slide" style="background-image:url('./images/banner4.png')"></div>
    </div>

    <div class="overlay">
      <div class="overlay-content">
        <h1>Enduring Icons of Luxury</h1>
        <button>EXPLORE COLLECTION</button>
      </div>
    </div>
  </div>

  <!-- Agentforce Demo -->
  <section>
    <h2>Ask Our Watch Advisor</h2>
    <p>
      AI-powered assistance for both collectors and partners — grounded in
      verified product and authentication knowledge.
    </p>

    <div class="agent-box">
      🤖 Agentforce Web Agent Demo Zone<br><br>
      • Answers from Salesforce Knowledge<br>
      • B2C & B2B ready<br>
      • Seamless escalation to experts
    </div>
  </section>

  <!-- Footer -->
  <footer>
    &copy; 2026 Demo Luxury Company. All rights reserved.
  </footer>

</body>
</html>
