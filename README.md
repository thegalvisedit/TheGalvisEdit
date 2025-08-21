<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>The Galvis Edit</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;700&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      font-family: 'Poppins', sans-serif;
      background: #f9f9f9;
      color: #333;
      overflow-x: hidden;
    }

    /* HERO SECTION */
    header {
      position: relative;
      height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: center;
      color: #fff;
      overflow: hidden;
    }
    header video {
      position: absolute;
      top: 0; left: 0;
      width: 100%;
      height: 100%;
      object-fit: cover;
      z-index: -1;
      filter: brightness(0.6);
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
      animation: fadeIn 2s ease;
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

    /* Services cards with images */
    .content-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 25px;
    }
    .card {
      background: #fff;
      border-radius: 20px;
      overflow: hidden;
      box-shadow: 0 6px 15px rgba(0,0,0,0.1);
      transition: transform 0.4s, box-shadow 0.4s;
      cursor: pointer;
      position: relative;
    }
    .card img {
      width: 100%;
      height: 200px;
      object-fit: cover;
      transition: transform 0.5s;
    }
    .card:hover img {
      transform: scale(1.1);
    }
    .card .card-text {
      padding: 15px;
      font-weight: 500;
      font-size: 1.2rem;
      text-align: center;
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
    }

    /* Animations */
    @keyframes fadeIn { from {opacity:0;} to {opacity:1;} }
    @keyframes slideDown { from {transform: translateY(-40px); opacity:0;} to {transform: translateY(0); opacity:1;} }
    @keyframes fadeUp { from {transform: translateY(40px); opacity:0;} to {transform: translateY(0); opacity:1;} }
    @keyframes growLine { from {width:0;} to {width:60px;} }

  </style>
</head>
<body>
  <header>
    <video autoplay muted loop>
      <source src="https://cdn.pixabay.com/vimeo/458313361/pexels-artem-podrez-458313361.mp4" type="video/mp4">
    </video>
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
      <div class="card">
        <img src="https://images.unsplash.com/photo-1505691723518-36a0d6d2e9c2?crop=entropy&cs=tinysrgb&fit=max&w=500" alt="Wedding">
        <div class="card-text">💍 Wedding Films & Photography</div>
      </div>
      <div class="card">
        <img src="https://images.unsplash.com/photo-1503676260728-1c00da094a0b?crop=entropy&cs=tinysrgb&fit=max&w=500" alt="Birthday">
        <div class="card-text">🎉 Birthday & Event Highlights</div>
      </div>
      <div class="card">
        <img src="https://images.unsplash.com/photo-1598970434795-0c54fe7c0642?crop=entropy&cs=tinysrgb&fit=max&w=500" alt="Gym">
        <div class="card-text">🏋️ Gym & Fitness Content</div>
      </div>
      <div class="card">
        <img src="https://images.unsplash.com/photo-1533750349088-cd871a92f312?crop=entropy&cs=tinysrgb&fit=max&w=500" alt="Business">
        <div class="card-text">🏢 Business & Brand Promotion</div>
      </div>
      <div class="card">
        <img src="https://images.unsplash.com/photo-1500917293891-ef795e70e1f6?crop=entropy&cs=tinysrgb&fit=max&w=500" alt="Photoshoot">
        <div class="card-text">📸 Professional Photoshoots</div>
      </div>
      <div class="card">
        <img src="https://images.unsplash.com/photo-1498050108023-c5249f4df085?crop=entropy&cs=tinysrgb&fit=max&w=500" alt="Social Media">
        <div class="card-text">🎬 Social Media Video Production</div>
      </div>
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
