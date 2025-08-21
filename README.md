<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>The Galvis Edit</title>
  <style>
    body {
      margin: 0;
      font-family: 'Poppins', sans-serif;
      background: #f9f9f9;
      color: #333;
      overflow-x: hidden;
    }
    header {
      height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: center;
      background: linear-gradient(135deg, #ff6a00, #ee0979);
      color: #fff;
      animation: fadeIn 2s ease-in;
      position: relative;
      overflow: hidden;
    }
    header h1 {
      font-size: 3.5rem;
      margin: 0;
      animation: slideDown 1.2s ease;
    }
    header p {
      font-size: 1.3rem;
      margin-top: 10px;
      opacity: 0.9;
      animation: fadeIn 2.5s ease;
    }
    header a {
      margin-top: 20px;
      display: inline-block;
      padding: 14px 28px;
      background: #fff;
      color: #ee0979;
      font-weight: bold;
      text-decoration: none;
      border-radius: 30px;
      transition: transform 0.3s, box-shadow 0.3s;
    }
    header a:hover {
      transform: scale(1.1);
      box-shadow: 0 6px 20px rgba(255,255,255,0.5);
    }

    section {
      padding: 70px 20px;
      max-width: 1100px;
      margin: auto;
      animation: fadeUp 1.5s ease;
    }

    h2 {
      text-align: center;
      margin-bottom: 30px;
      font-size: 2.2rem;
      color: #222;
      position: relative;
    }
    h2::after {
      content: "";
      width: 60px;
      height: 4px;
      background: #ee0979;
      display: block;
      margin: 10px auto 0;
      border-radius: 2px;
      animation: growLine 1.5s ease forwards;
    }

    .about p {
      text-align: center;
      font-size: 1.1rem;
      line-height: 1.7;
    }

    .content-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 25px;
    }

    .card {
      background: #fff;
      border-radius: 20px;
      padding: 25px;
      box-shadow: 0 6px 15px rgba(0,0,0,0.1);
      text-align: center;
      font-size: 1.2rem;
      font-weight: 500;
      transition: transform 0.4s, box-shadow 0.4s;
      animation: popIn 1s ease;
    }
    .card:hover {
      transform: translateY(-12px) scale(1.05);
      box-shadow: 0 12px 25px rgba(0,0,0,0.2);
    }

    .contact p {
      text-align: center;
      font-size: 1.1rem;
    }

    footer {
      text-align: center;
      padding: 20px;
      background: #ee0979;
      color: #fff;
      position: relative;
    }

    /* Animations */
    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }
    @keyframes slideDown {
      from { transform: translateY(-40px); opacity: 0; }
      to { transform: translateY(0); opacity: 1; }
    }
    @keyframes fadeUp {
      from { transform: translateY(40px); opacity: 0; }
      to { transform: translateY(0); opacity: 1; }
    }
    @keyframes growLine {
      from { width: 0; }
      to { width: 60px; }
    }
    @keyframes popIn {
      0% { transform: scale(0.8); opacity: 0; }
      100% { transform: scale(1); opacity: 1; }
    }

    /* Floating circles background effect */
    .circle {
      position: absolute;
      border-radius: 50%;
      background: rgba(255,255,255,0.2);
      animation: float 10s infinite;
    }
    .circle.small { width: 40px; height: 40px; bottom: 10%; left: 20%; }
    .circle.medium { width: 70px; height: 70px; bottom: 20%; right: 15%; }
    .circle.large { width: 120px; height: 120px; top: 15%; left: 10%; }

    @keyframes float {
      0% { transform: translateY(0) rotate(0deg); }
      50% { transform: translateY(-30px) rotate(180deg); }
      100% { transform: translateY(0) rotate(360deg); }
    }
  </style>
</head>
<body>
  <header>
    <div class="circle small"></div>
    <div class="circle medium"></div>
    <div class="circle large"></div>
    <h1>The Galvis Edit ✨</h1>
    <p>We create content that makes your moments unforgettable.<br>Weddings · Birthdays · Gyms · Businesses & more</p>
    <a href="#about">Discover Our Work</a>
  </header>

  <section id="about" class="about">
    <h2>About Us</h2>
    <p>The Galvis Edit specializes in creating impactful visual stories. Whether it’s capturing the magic of a wedding, the energy of a gym, or helping businesses shine online, we bring creativity and innovation to every project.</p>
  </section>

  <section class="content">
    <h2>Our Services</h2>
    <div class="content-grid">
      <div class="card">💍 Wedding Films & Photography</div>
      <div class="card">🎉 Birthday & Event Highlights</div>
      <div class="card">🏋️ Gym & Fitness Content</div>
      <div class="card">🏢 Business & Brand Promotion</div>
      <div class="card">📸 Professional Photoshoots</div>
      <div class="card">🎬 Social Media Video Production</div>
    </div>
  </section>

  <section class="contact">
    <h2>Contact Us</h2>
    <p>Ready to bring your vision to life? Let’s collaborate!</p>
    <p>📧 contact@thegalvisedit.com</p>
  </section>

  <footer>
    <p>© 2025 The Galvis Edit | Follow us on 🌐 Instagram · YouTube · TikTok</p>
  </footer>
</body>
</html>
