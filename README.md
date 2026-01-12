
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Luxury Watches & Jewelry | Demo</title>

  <style>
    :root {
      --black: #0b0b0b;
      --dark: #121212;
      --light: #f5f5f5;
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
      color: #ffffff;
      line-height: 1.6;
    }

    /* Header */
    header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 24px 48px;
      border-bottom: 1px solid #1f1f1f;
    }

    .logo {
      font-size: 1.6rem;
      font-weight: 500;
      letter-spacing: 1px;
    }

    nav a {
      color: var(--muted);
      text-decoration: none;
      margin-left: 28px;
      font-size: 0.95rem;
    }

    nav a:hover {
      color: var(--gold);
    }

    /* Hero */
    .hero {
      padding: 110px 40px;
      text-align: center;
      background: linear-gradient(to bottom, #151515, #0b0b0b);
    }

    .hero h1 {
      font-size: 3rem;
      font-weight: 300;
      margin-bottom: 20px;
    }

    .hero p {
      max-width: 720px;
      margin: auto;
      font-size: 1.1rem;
      color: var(--muted);
    }

    /* Sections */
    section {
      padding: 80px 40px;
    }

    section.light {
      background: var(--light);
      color: #111;
    }

    h2 {
      text-align: center;
      font-weight: 400;
      font-size: 2rem;
      margin-bottom: 48px;
    }

    /* Cards */
    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 32px;
      max-width: 1100px;
      margin: auto;
    }

    .card {
      border: 1px solid #222;
      padding: 36px 28px;
      text-align: center;
      transition: all 0.3s ease;
    }

    .light .card {
      border-color: #ddd;
    }

    .card:hover {
      transform: translateY(-6px);
      border-color: var(--gold);
    }

    .card h3 {
      margin-bottom: 12px;
      font-weight: 500;
    }

    .card p {
      color: var(--muted);
      font-size: 0.95rem;
    }

    .light .card p {
      color: #444;
    }

    /* AI Demo */
    .ai-demo {
      max-width: 820px;
      margin: auto;
      text-align: center;
    }

    .ai-demo p {
      color: var(--muted);
      margin-bottom: 28px;
    }

    .agent-box {
      border: 2px dashed var(--gold);
      padding: 44px;
      border-radius: 6px;
      font-size: 0.95rem;
    }

    /* Footer */
    footer {
      padding: 48px;
      text-align: center;
      border-top: 1px solid #1f1f1f;
      color: var(--muted);
      font-size: 0.85rem;
    }

    footer a {
      color: var(--muted);
      text-decoration: none;
      margin: 0 10px;
    }

    footer a:hover {
      color: var(--gold);
    }

    /* Mobile */
    @media (max-width: 768px) {
      nav {
        display: none;
      }

      .hero h1 {
        font-size: 2.2rem;
      }
    }
  </style>
</head>

<body>

  <!-- Header -->
  <header>
    <div class="logo">Demo Luxury</div>
    <nav>
      <a href="#">Watches</a>
      <a href="#">Jewelry</a>
      <a href="#">Pre-Owned</a>
      <a href="#">Sell & Trade</a>
      <a href="#">Contact</a>
    </nav>
  </header>

  <!-- Hero -->
  <div class="hero">
    <h1>Exceptional Watches & Fine Jewelry</h1>
    <p>
      Curated luxury timepieces and jewelry trusted by collectors,
      enthusiasts, and global partners.
    </p>
  </div>

  <!-- Brands -->
  <section>
    <h2>Featured Brands</h2>
    <div class="grid">
      <div class="card"><h3>Rolex</h3><p>Iconic precision and heritage</p></div>
      <div class="card"><h3>Patek Philippe</h3><p>Generational craftsmanship</p></div>
      <div class="card"><h3>Cartier</h3><p>Timeless elegance</p></div>
      <div class="card"><h3>Omega</h3><p>Innovation and legacy</p></div>
    </div>
  </section>

  <!-- Collections -->
  <section class="light">
    <h2>Our Collections</h2>
    <div class="grid">
      <div class="card"><h3>New Arrivals</h3><p>Latest acquisitions</p></div>
      <div class="card"><h3>Pre-Owned Watches</h3><p>Certified and authenticated</p></div>
      <div class="card"><h3>Fine Jewelry</h3><p>Exceptional craftsmanship</p></div>
      <div class="card"><h3>Sell & Trade</h3><p>Trusted global marketplace</p></div>
    </div>
  </section>

  <!-- AI Agent Demo -->
  <section>
    <h2>Ask Our Watch Advisor</h2>
    <div class="ai-demo">
      <p>
        Our AI-powered advisor assists both consumers and partners
        with product knowledge, authentication, and buying guidance — 24/7.
      </p>

      <div class="agent-box">
        🤖 Agentforce Web Agent Demo Zone<br/><br/>
        • Answers from verified Salesforce Knowledge<br/>
        • Supports B2C & B2B inquiries<br/>
        • Seamless escalation to human experts
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer>
    <p>&copy; 2026 Demo Luxury Company. All rights reserved.</p>
    <p>
      <a href="#">Privacy</a> |
      <a href="#">Terms</a>
    </p>
  </footer>

</body>
</html>
