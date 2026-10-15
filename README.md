
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Aditya Singh | BMW Experience</title>

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: Arial, sans-serif;
      background: #080b10;
      color: white;
    }

    header {
      height: 80px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 0 7%;
      background: rgba(0, 0, 0, 0.85);
      border-bottom: 1px solid #292d35;
    }

    .logo {
      font-size: 27px;
      font-weight: bold;
      color: #49a5ff;
      letter-spacing: 3px;
    }

    nav a {
      color: white;
      text-decoration: none;
      margin-left: 25px;
      font-size: 14px;
      transition: 0.3s;
    }

    nav a:hover {
      color: #49a5ff;
    }

    .hero {
      min-height: 85vh;
      display: flex;
      align-items: center;
      padding: 70px 8%;
      background:
        linear-gradient(90deg, #080b10 5%, rgba(8,11,16,.85) 38%, transparent 100%),
        url("https://images.unsplash.com/photo-1555215695-3004980ad54e?auto=format&fit=crop&w=1800&q=85")
        center / cover no-repeat;
    }

    .hero-content {
      max-width: 580px;
    }

    .tag {
      color: #49a5ff;
      letter-spacing: 4px;
      font-size: 13px;
      margin-bottom: 22px;
    }

    h1 {
      font-size: clamp(42px, 7vw, 76px);
      line-height: 1.05;
      margin-bottom: 24px;
    }

    h1 span {
      color: #49a5ff;
    }

    .description {
      color: #c5c9d0;
      line-height: 1.8;
      max-width: 470px;
      margin-bottom: 32px;
    }

    .btn {
      display: inline-block;
      background: #1674e8;
      color: white;
      border: none;
      padding: 15px 25px;
      text-decoration: none;
      cursor: pointer;
      font-size: 14px;
      font-weight: bold;
      transition: 0.3s;
    }

    .btn:hover {
      background: #49a5ff;
      transform: translateY(-3px);
    }

    .secondary {
      background: transparent;
      border: 1px solid white;
      margin-left: 10px;
    }

    .models {
      padding: 70px 8%;
      text-align: center;
    }

    .models h2 {
      font-size: 35px;
      margin-bottom: 12px;
    }

    .models > p {
      color: #aeb5c0;
      margin-bottom: 35px;
    }

    .car-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 22px;
      text-align: left;
    }

    .car-card {
      background: #141922;
      border: 1px solid #252c38;
      transition: 0.3s;
    }

    .car-card:hover {
      transform: translateY(-7px);
      border-color: #49a5ff;
    }

    .car-card img {
      width: 100%;
      height: 210px;
      object-fit: cover;
    }

    .car-info {
      padding: 22px;
    }

    .car-info h3 {
      margin-bottom: 10px;
    }

    .car-info p {
      color: #aeb5c0;
      font-size: 14px;
      line-height: 1.6;
      margin-bottom: 18px;
    }

    .car-info button {
      width: 100%;
    }

    footer {
      padding: 25px;
      text-align: center;
      color: #9299a5;
      border-top: 1px solid #292d35;
      font-size: 13px;
    }

    @media (max-width: 760px) {
      header {
        padding: 20px 5%;
        height: auto;
        flex-direction: column;
        gap: 18px;
      }

      nav {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        gap: 15px;
      }

      nav a {
        margin: 0;
      }

      .hero {
        min-height: 75vh;
        padding: 55px 6%;
        background-position: 60% center;
      }

      .hero-content {
        background: rgba(8, 11, 16, 0.55);
        padding: 12px 0;
      }

      .car-grid {
        grid-template-columns: 1fr;
      }

      .secondary {
        margin: 12px 0 0;
      }
    }
  </style>
</head>

<body>

  <header>
    <div class="logo">BMW</div>

    <nav>
      <a href="#home">Home</a>
      <a href="#models">Models</a>
      <a href="#about">About</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <section class="hero" id="home">
    <div class="hero-content">
      <p class="tag">SHEER DRIVING PLEASURE</p>

      <h1>THE ULTIMATE<br><span>DRIVING</span><br>MACHINE.</h1>

      <p class="description">
        Experience bold design, incredible performance
        and the thrill of driving. Discover the world
        of BMW with Aditya Singh.
      </p>

      <a href="#models" class="btn">EXPLORE MODELS</a>
      <a href="#about" class="btn secondary">DISCOVER MORE</a>
    </div>
  </section>

  <section class="models" id="models">
    <h2>Explore Our Models</h2>
    <p>Find the BMW that matches your personality.</p>

    <div class="car-grid">

      <div class="car-card">
        <img
          src="https://images.unsplash.com/photo-1555215695-3004980ad54e?auto=format&fit=crop&w=800&q=80"
          alt="Luxury BMW sedan">
        <div class="car-info">
          <h3>BMW 3 Series</h3>
          <p>Sporty styling and a refined driving experience.</p>
          <button class="btn" onclick="showDetails('BMW 3 Series')">
            VIEW DETAILS
          </button>
        </div>
      </div>

      <div class="car-card">
        <img
          src="https://images.unsplash.com/photo-1556189250-72ba954cfc2b?auto=format&fit=crop&w=800&q=80"
          alt="BMW luxury car">
        <div class="car-info">
          <h3>BMW M Series</h3>
          <p>Powerful performance with a bold, athletic character.</p>
          <button class="btn" onclick="showDetails('BMW M Series')">
            VIEW DETAILS
          </button>
        </div>
      </div>

      <div class="car-card">
        <img
          src="https://images.unsplash.com/photo-1511919884226-fd3cad34687c?auto=format&fit=crop&w=800&q=80"
          alt="Premium sports car">
        <div class="car-info">
          <h3>BMW Luxury</h3>
          <p>Modern design and premium comfort for every journey.</p>
          <button class="btn" onclick="showDetails('BMW Luxury')">
            VIEW DETAILS
          </button>
        </div>
      </div>

    </div>
  </section>

  <section class="models" id="about">
    <h2>Designed for Driving Enthusiasts</h2>
    <p>
      Created by Aditya Singh — a personal BMW-inspired
      website concept celebrating luxury and performance.
    </p>
  </section>

  <footer id="contact">
    <p>© 2026 Aditya Singh | BMW-Inspired Website Project</p>
    <p style="margin-top: 10px;">
      Independent fan project. Not an official BMW website.
    </p>
  </footer>

  <script>
    function showDetails(model) {
      alert(
        "You selected " + model +
        "! Thanks for visiting Aditya Singh's website."
      );
    }
  </script>

</body>
</html>
