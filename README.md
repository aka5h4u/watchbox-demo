<html>
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Luxury Watches & Jewelry | WatchBox Demo</title>

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
	  .category-section {
  padding: 80px 40px;
  background: #111; /* slightly lighter than body */
  border: 2px solid red; /* DEBUG BORDER */
}

    /* Hero Banner Rotation */
    .hero {
  position: relative;
  width: 100vw;          /* FORCE full viewport width */
  height: 80vh;
  overflow: hidden;
  margin-left: calc(-50vw + 50%); /* prevents body padding issues */
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

  <!-- Header  -->
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
      <div class="slide" style="background-image: url('Banner6.png')"></div>
      <div class="slide" style="background-image: url('Banner5.png')"></div>
      <div class="slide" style="background-image: url('Banner7.png')"></div>
      <div class="slide" style="background-image: url('Banner8.png')"></div>
    </div>

    <div class="hero-overlay">
      <div class="hero-content">
        <h1>Timeless Icons of Luxury</h1>
        <button>EXPLORE COLLECTION</button>
      </div>
    </div>
  </div>
  <!-- Couples & Gifts Section -->
<section class="category-section">
  <div class="category-grid">

    <div class="category-card">
      <img src="Couples.png" alt="Couples Collection">
      <div class="category-overlay">
        <h3>Couples</h3>
      </div>
    </div>

    <div class="category-card">
      <img src="Gifts.png" alt="Gifts Collection">
      <div class="category-overlay">
        <h3>Gifts</h3>
      </div>
    </div>

  </div>
</section>

  <!-- Agentforce Demo Section -->
  <section>
    <h2>Ask Our Watch Advisor</h2>
    <p>
      AI-powered guidance for collectors and partners — grounded in trusted
      product and authentication knowledge.
    </p>

    <div class="agent-demo">
      🤖 Agentforce Web Agent Demo Area [13/01/2026]<br><br>
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
  <script type='text/javascript'>
	function initEmbeddedMessaging() {
		try {
			embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'

			embeddedservice_bootstrap.init(
				'00Dfj00000GhufN',
				'Github_Messaging_Setting',
				'https://orgfarm-23fcbe497c-dev-ed.develop.my.site.com/ESWGithubMessagingSetti1768249695612',
				{
					scrt2URL: 'https://orgfarm-23fcbe497c-dev-ed.develop.my.salesforce-scrt.com'
				}
			);
		} catch (err) {
			console.error('Error loading Embedded Messaging: ', err);
		}
	};
	</script>
	<script type='text/javascript' src='https://orgfarm-23fcbe497c-dev-ed.develop.my.site.com/ESWGithubMessagingSetti1768249695612/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>


</body>
</html>
