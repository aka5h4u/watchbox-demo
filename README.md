<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Luxury Watches & Jewelry | Demo</title>

  <style>
    :root {
      --bg-dark: #0c0c0c;
      --bg-light: #f7f7f7;
      --text-light: #ffffff;
      --text-muted: #bbbbbb;
      --accent: #c9a14a;
    }

    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      font-family: "Helvetica Neue", Arial, sans-serif;
      background: var(--bg-dark);
      color: var(--text-light);
      line-height: 1.6;
    }

    /* Header */
    header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 20px 40px;
      border-bottom: 1px solid #222;
    }

    header .logo {
      font-size: 1.6rem;
      font-weight: 600;
      letter-spacing: 1px;
    }

    nav a {
      color: var(--text-muted);
      text-decoration: none;
      margin-left: 24px;
      font-size: 0.95rem;
    }

    nav a:hover {
      color: var(--accent);
    }

    /* Hero */
    .hero {
      padding: 100px 40px;
      text-align: center;
      background: linear-gradient(to bottom, #111, #000);
    }

    .hero h1 {
      font-size: 3rem;
      font-weight: 300;
      margin-bottom: 20px;
    }

    .hero p {
      max-width: 700px;
      margin: 0 auto;
      color: var(--text-muted);
      font-size: 1.1rem;
    }

    /* Sections */
    .section {
      padding: 80px 40px;
      background: var(--bg-dark);
    }

    .section.light {
      background: var(--bg-light);
      color: #111;
    }

    .section h2 {
      text-align: center;
      font-weight: 400;
      font-size: 2rem;
      margin-bottom: 40px;
    }

    /* Cards */
    .card-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 30px;
      max-width: 1100px;
      margin: auto;
    }

    .card {
      border: 1px solid #222;
      padding: 30px;
      text-align: center;
      transition: all 0.3s ease;
    }

    .section.light .card {
      border-color: #ddd;
    }

    .card:hover {
      transform: translateY(-6px);
      border-color: var(--accent);
    }

    .card h3 {
      margin-bottom: 10px;
      font-weight: 500;
    }

    .card p {
      color: var(--text-muted);
      font-size: 0.95rem;
    }

    .section.light .card p {
      color: #444;
    }

    /* AI Demo Section */
    .ai-demo {
      text-align: center;
      max-width: 800px;
      margin: auto;
    }

    .ai-demo p {
      color: var(--text-muted);
      margin-bottom: 30px;
    }

    .ai-placeholder {
      border: 2px dashed var(--accent);
      padding: 40px;
      border-radius: 6px;
      font-size: 0.95rem;
    }

    /* Footer */
    footer {
      padding: 40px;
      text-align: center;
      border-top: 1px solid #222;
      color: var(--text-muted);
      font-size: 0.85rem;
    }

    footer a {
      color: var(--text-muted);
      text-decoration: none;
      margin: 0 10px;
    }

    footer a:hover {
      color: var(--accent);
    }

    /* Responsive */
    @media (max-width: 768px) {
      .hero h1 {
        font-size: 2.2rem;
      }
      nav {
        display: none;
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
  <section class="hero">
    <h1>Exceptional Watches & Fine Jewelry</h1>
    <p>
      Discover curated timepieces and jewelry trusted by collectors, enthusiasts,
      and global partners.
    </p>
  </section>

  <!-- Brands -->
  <section class="section">
    <h2>Featured Brands</h2>
    <div class="card-grid">
      <div class="card"><h3>Rolex</h3><p>Iconic precision & heritage</p></div>
      <div class="card"><h3>Patek Philippe</h3><p>Generational craftsmanship</p></div>
      <div class="card"><h3>Cartier</h3><p>Timeless elegance</p></div>
      <div class="card"><h3>Omega</h3><p>Innovation & legacy</p></div>
    </div>
  </section>

  <!-- Collections -->
  <section class="section light">
    <h2>Our Collections</h2>
    <div class="card-grid">
      <div class="card"><h3>New Arrivals</h3><p>Latest acquisitions</p></div>
      <div class="card"><h3>Pre-Owned</h3><p>Certified luxury watches</p></div>
      <div class="card"><h3>Fine Jewelry</h3><p>Exceptional craftsmanship</p></div>
      <div class="card"><h3>Sell & Trade</h3><p>Trusted global marketplace</p></div>
    </div>
  </section>

  <!-- AI Agent Demo -->
  <section class="section">
    <h2>Ask Our Watch Advisor</h2>
    <div class="ai-demo">
      <p>
        Our AI-powered advisor helps clients and partners with product questions,
        authentication guidance, and buying decisions — 24/7.
      </p>

      <div class="ai-placeholder">
        🤖 Agentforce Web Agent Placeholder<br/><br/>
        • Answers from verified Knowledge Articles<br/>
        • Supports both B2C & B2B inquiries<br/>
        • Seamless handoff to human experts
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
