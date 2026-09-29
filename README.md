<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>YourDesireServices | Professional Multi-Purpose Services</title>

  <meta
    name="description"
    content="YourDesireServices provides reliable, professional, and convenient services tailored to your needs."
  >

  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

  <link
    href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap"
    rel="stylesheet"
  >

  <style>
    :root {
      --primary: #2563eb;
      --primary-dark: #1d4ed8;
      --secondary: #0f172a;
      --text: #334155;
      --muted: #64748b;
      --light: #f8fafc;
      --white: #ffffff;
      --border: #e2e8f0;
      --success: #10b981;
      --shadow: 0 15px 40px rgba(15, 23, 42, 0.08);
      --radius: 18px;
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      font-family: "Inter", sans-serif;
      color: var(--text);
      background: var(--white);
      line-height: 1.6;
    }

    a {
      text-decoration: none;
      color: inherit;
    }

    img {
      max-width: 100%;
      display: block;
    }

    .container {
      width: min(1120px, 92%);
      margin: auto;
    }

    /* =========================
       NAVIGATION
    ========================= */

    header {
      position: fixed;
      top: 0;
      width: 100%;
      z-index: 1000;
      background: rgba(255, 255, 255, 0.94);
      backdrop-filter: blur(12px);
      border-bottom: 1px solid rgba(226, 232, 240, 0.8);
    }

    .navbar {
      height: 76px;
      display: flex;
      align-items: center;
      justify-content: space-between;
    }

    .logo {
      font-size: 1.35rem;
      font-weight: 800;
      color: var(--secondary);
      letter-spacing: -0.5px;
    }

    .logo span {
      color: var(--primary);
    }

    .nav-links {
      display: flex;
      align-items: center;
      gap: 30px;
      list-style: none;
    }

    .nav-links a {
      font-size: 0.92rem;
      font-weight: 600;
      color: var(--text);
      transition: 0.3s;
    }

    .nav-links a:hover {
      color: var(--primary);
    }

    .nav-button {
      padding: 11px 20px;
      background: var(--primary);
      color: white !important;
      border-radius: 9px;
    }

    .nav-button:hover {
      background: var(--primary-dark);
    }

    .menu-toggle {
      display: none;
      border: none;
      background: transparent;
      font-size: 1.7rem;
      cursor: pointer;
      color: var(--secondary);
    }

    /* =========================
       HERO
    ========================= */

    .hero {
      padding: 170px 0 100px;
      background:
        radial-gradient(circle at 85% 20%, rgba(37, 99, 235, 0.13), transparent 30%),
        radial-gradient(circle at 10% 80%, rgba(14, 165, 233, 0.08), transparent 25%),
        var(--light);
    }

    .hero-content {
      display: grid;
      grid-template-columns: 1.1fr 0.9fr;
      gap: 60px;
      align-items: center;
    }

    .hero-badge {
      display: inline-flex;
      align-items: center;
      gap: 8px;
      background: #eff6ff;
      color: var(--primary);
      padding: 8px 14px;
      border-radius: 30px;
      font-size: 0.85rem;
      font-weight: 700;
      margin-bottom: 22px;
    }

    .hero-badge::before {
      content: "";
      width: 8px;
      height: 8px;
      background: var(--success);
      border-radius: 50%;
    }

    .hero h1 {
      font-size: clamp(2.5rem, 5vw, 4.5rem);
      line-height: 1.05;
      letter-spacing: -2.5px;
      color: var(--secondary);
      margin-bottom: 24px;
    }

    .hero h1 span {
      color: var(--primary);
    }

    .hero p {
      max-width: 620px;
      font-size: 1.08rem;
      color: var(--muted);
      margin-bottom: 32px;
    }

    .hero-buttons {
      display: flex;
      gap: 14px;
      flex-wrap: wrap;
    }

    .btn {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      padding: 14px 23px;
      border-radius: 10px;
      font-weight: 700;
      transition: 0.3s;
      border: 2px solid transparent;
    }

    .btn-primary {
      background: var(--primary);
      color: white;
      box-shadow: 0 10px 25px rgba(37, 99, 235, 0.25);
    }

    .btn-primary:hover {
      background: var(--primary-dark);
      transform: translateY(-2px);
    }

    .btn-outline {
      border-color: var(--border);
      background: white;
      color: var(--secondary);
    }

    .btn-outline:hover {
      border-color: var(--primary);
      color: var(--primary);
    }

    /* Hero Card */

    .hero-card {
      position: relative;
      background: white;
      border-radius: 24px;
      padding: 35px;
      box-shadow: var(--shadow);
      border: 1px solid var(--border);
    }

    .hero-card-icon {
      width: 65px;
      height: 65px;
      display: flex;
      align-items: center;
      justify-content: center;
      background: #eff6ff;
      color: var(--primary);
      border-radius: 16px;
      font-size: 1.8rem;
      margin-bottom: 25px;
    }

    .hero-card h3 {
      color: var(--secondary);
      font-size: 1.4rem;
      margin-bottom: 10px;
    }

    .hero-card p {
      font-size: 0.95rem;
      margin-bottom: 25px;
    }

    .hero-list {
      list-style: none;
    }

    .hero-list li {
      display: flex;
      gap: 10px;
      align-items: center;
      margin: 13px 0;
      font-size: 0.92rem;
      font-weight: 600;
    }

    .hero-list li::before {
      content: "✓";
      display: flex;
      align-items: center;
      justify-content: center;
      width: 22px;
      height: 22px;
      background: #dcfce7;
      color: #16a34a;
      border-radius: 50%;
      font-size: 0.75rem;
      font-weight: 800;
    }

    /* =========================
       GENERAL SECTIONS
    ========================= */

    section {
      padding: 95px 0;
    }

    .section-header {
      text-align: center;
      max-width: 680px;
      margin: 0 auto 55px;
    }

    .section-label {
      color: var(--primary);
      font-size: 0.82rem;
      font-weight: 800;
      text-transform: uppercase;
      letter-spacing: 1.5px;
      margin-bottom: 12px;
    }

    .section-header h2 {
      color: var(--secondary);
      font-size: clamp(2rem, 4vw, 3rem);
      line-height: 1.15;
      letter-spacing: -1px;
      margin-bottom: 15px;
    }

    .section-header p {
      color: var(--muted);
    }

    /* =========================
       SERVICES
    ========================= */

    .services {
      background: white;
    }

    .services-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 22px;
    }

    .service-card {
      padding: 30px;
      border: 1px solid var(--border);
      border-radius: var(--radius);
      transition: 0.3s;
      background: white;
    }

    .service-card:hover {
      transform: translateY(-7px);
      box-shadow: var(--shadow);
      border-color: #bfdbfe;
    }

    .service-icon {
      width: 54px;
      height: 54px;
      border-radius: 14px;
      background: #eff6ff;
      color: var(--primary);
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 1.45rem;
      margin-bottom: 20px;
    }

    .service-card h3 {
      color: var(--secondary);
      margin-bottom: 10px;
      font-size: 1.15rem;
    }

    .service-card p {
      color: var(--muted);
      font-size: 0.92rem;
    }

    /* =========================
       ABOUT
    ========================= */

    .about {
      background: var(--light);
    }

    .about-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 70px;
      align-items: center;
    }

    .about-image {
      min-height: 420px;
      border-radius: 25px;
      background:
        linear-gradient(135deg, rgba(37, 99, 235, 0.9), rgba(15, 23, 42, 0.9)),
        linear-gradient(45deg, #2563eb, #0f172a);
      display: flex;
      align-items: center;
      justify-content: center;
      color: white;
      position: relative;
      overflow: hidden;
    }

    .about-image::before {
      content: "";
      position: absolute;
      width: 250px;
      height: 250px;
      border: 50px solid rgba(255,255,255,0.08);
      border-radius: 50%;
    }

    .about-logo {
      z-index: 1;
      text-align: center;
    }

    .about-logo strong {
      display: block;
      font-size: 2.2rem;
      letter-spacing: -1px;
    }

    .about-logo span {
      color: #bfdbfe;
    }

    .about-content .section-label {
      margin-bottom: 12px;
    }

    .about-content h2 {
      color: var(--secondary);
      font-size: 2.5rem;
      line-height: 1.15;
      margin-bottom: 20px;
    }

    .about-content > p {
      color: var(--muted);
      margin-bottom: 25px;
    }

    .check-list {
      list-style: none;
    }

    .check-list li {
      display: flex;
      gap: 12px;
      margin: 14px 0;
      font-weight: 600;
    }

    .check-list li span {
      color: var(--success);
      font-weight: 900;
    }

    /* =========================
       WHY US
    ========================= */

    .features-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 30px;
    }

    .feature {
      text-align: center;
      padding: 25px;
    }

    .feature-number {
      width: 60px;
      height: 60px;
      margin: 0 auto 20px;
      border-radius: 50%;
      background: #eff6ff;
      color: var(--primary);
      display: flex;
      align-items: center;
      justify-content: center;
      font-weight: 800;
      font-size: 1.2rem;
    }

    .feature h3 {
      color: var(--secondary);
      margin-bottom: 10px;
    }

    .feature p {
      color: var(--muted);
      font-size: 0.92rem;
    }

    /* =========================
       CTA
    ========================= */

    .cta {
      padding: 75px 0;
    }

    .cta-box {
      background: var(--secondary);
      border-radius: 25px;
      padding: 65px;
      text-align: center;
      color: white;
      position: relative;
      overflow: hidden;
    }

    .cta-box::before,
    .cta-box::after {
      content: "";
      position: absolute;
      border-radius: 50%;
      background: rgba(37, 99, 235, 0.2);
    }

    .cta-box::before {
      width: 250px;
      height: 250px;
      top: -120px;
      left: -80px;
    }

    .cta-box::after {
      width: 300px;
      height: 300px;
      bottom: -170px;
      right: -100px;
    }

    .cta-content {
      position: relative;
      z-index: 1;
    }

    .cta-box h2 {
      font-size: clamp(2rem, 4vw, 3rem);
      margin-bottom: 15px;
    }

    .cta-box p {
      max-width: 620px;
      margin: 0 auto 28px;
      color: #cbd5e1;
    }

    /* =========================
       CONTACT
    ========================= */

    .contact {
      background: var(--light);
    }

    .contact-grid {
      display: grid;
      grid-template-columns: 0.8fr 1.2fr;
      gap: 45px;
    }

    .contact-info h2 {
      color: var(--secondary);
      font-size: 2.3rem;
      margin-bottom: 15px;
    }

    .contact-info > p {
      color: var(--muted);
      margin-bottom: 30px;
    }

    .contact-item {
      display: flex;
      gap: 15px;
      margin: 20px 0;
    }

    .contact-item-icon {
      width: 45px;
      height: 45px;
      border-radius: 10px;
      background: white;
      display: flex;
      align-items: center;
      justify-content: center;
      color: var(--primary);
      border: 1px solid var(--border);
    }

    .contact-item strong {
      display: block;
      color: var(--secondary);
      margin-bottom: 3px;
    }

    .contact-item span {
      color: var(--muted);
      font-size: 0.9rem;
    }

    .contact-form {
      background: white;
      padding: 35px;
      border-radius: 20px;
      border: 1px solid var(--border);
      box-shadow: var(--shadow);
    }

    .form-group {
      margin-bottom: 18px;
    }

    .form-group label {
      display: block;
      font-size: 0.85rem;
      font-weight: 700;
      color: var(--secondary);
      margin-bottom: 7px;
    }

    .form-group input,
    .form-group textarea,
    .form-group select {
      width: 100%;
      padding: 13px 15px;
      border: 1px solid var(--border);
      border-radius: 9px;
      font-family: inherit;
      font-size: 0.92rem;
      outline: none;
      transition: 0.3s;
    }

    .form-group input:focus,
    .form-group textarea:focus,
    .form-group select:focus {
      border-color: var(--primary);
      box-shadow: 0 0 0 3px rgba(37, 99, 235, 0.1);
    }

    .form-group textarea {
      min-height: 130px;
      resize: vertical;
    }

    .submit-btn {
      width: 100%;
      border: none;
      cursor: pointer;
      font-family: inherit;
    }

    /* =========================
       FOOTER
    ========================= */

    footer {
      background: #020617;
      color: #94a3b8;
      padding: 55px 0 25px;
    }

    .footer-grid {
      display: grid;
      grid-template-columns: 1.5fr 1fr 1fr;
      gap: 50px;
      padding-bottom: 40px;
    }

    .footer-logo {
      color: white;
      font-size: 1.4rem;
      font-weight: 800;
      margin-bottom: 15px;
    }

    .footer-logo span {
      color: #60a5fa;
    }

    .footer-description {
      max-width: 380px;
      font-size: 0.9rem;
    }

    .footer-column h4 {
      color: white;
      margin-bottom: 17px;
    }

    .footer-column ul {
      list-style: none;
    }

    .footer-column li {
      margin: 10px 0;
      font-size: 0.9rem;
    }

    .footer-column a:hover {
      color: white;
    }

    .footer-bottom {
      padding-top: 25px;
      border-top: 1px solid #1e293b;
      text-align: center;
      font-size: 0.82rem;
    }

    /* =========================
       ANIMATION
    ========================= */

    .fade-up {
      animation: fadeUp 0.8s ease forwards;
    }

    @keyframes fadeUp {
      from {
        opacity: 0;
        transform: translateY(20px);
      }

      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    /* =========================
       RESPONSIVE
    ========================= */

    @media (max-width: 900px) {

      .hero-content,
      .about-grid,
      .contact-grid {
        grid-template-columns: 1fr;
      }

      .services-grid,
      .features-grid {
        grid-template-columns: repeat(2, 1fr);
      }

      .hero {
        padding-top: 135px;
      }

      .hero-card {
        max-width: 600px;
      }

      .about-image {
        min-height: 330px;
      }

      .footer-grid {
        grid-template-columns: 1fr 1fr;
      }
    }

    @media (max-width: 650px) {

      .navbar {
        height: 68px;
      }

      .menu-toggle {
        display: block;
      }

      .nav-links {
        position: absolute;
        top: 68px;
        left: 0;
        width: 100%;
        background: white;
        flex-direction: column;
        align-items: flex-start;
        padding: 25px;
        gap: 18px;
        border-bottom: 1px solid var(--border);
        display: none;
      }

      .nav-links.active {
        display: flex;
      }

      .nav-button {
        width: 100%;
        text-align: center;
      }

      .hero {
        padding: 120px 0 75px;
      }

      .hero h1 {
        letter-spacing: -1.5px;
      }

      section {
        padding: 70px 0;
      }

      .services-grid,
      .features-grid {
        grid-template-columns: 1fr;
      }

      .cta-box {
        padding: 45px 25px;
      }

      .contact-form {
        padding: 25px;
      }

      .footer-grid {
        grid-template-columns: 1fr;
        gap: 30px;
      }
    }
  </style>
</head>

<body>

  <!-- =========================
       HEADER
  ========================= -->

  <header>
    <div class="container navbar">

      <a href="#home" class="logo">
        YourDesire<span>Services</span>
      </a>

      <button class="menu-toggle" id="menuToggle" aria-label="Open menu">
        ☰
      </button>

      <ul class="nav-links" id="navLinks">
        <li><a href="#home">Home</a></li>
        <li><a href="#services">Services</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#contact">Contact</a></li>
        <li>
          <a href="#contact" class="nav-button">Get Started</a>
        </li>
      </ul>

    </div>
  </header>


  <!-- =========================
       HERO
  ========================= -->

  <main>

    <section class="hero" id="home">

      <div class="container hero-content">

        <div class="fade-up">

          <div class="hero-badge">
            Professional Services You Can Trust
          </div>

          <h1>
            Services Designed Around
            <span>Your Desires.</span>
          </h1>

          <p>
            YourDesireServices provides dependable, professional,
            and convenient solutions for individuals, families,
            and businesses. Whatever you need, we're here to help.
          </p>

          <div class="hero-buttons">

            <a href="#services" class="btn btn-primary">
              Explore Services
            </a>

            <a href="#contact" class="btn btn-outline">
              Contact Us
            </a>

          </div>

        </div>


        <div class="hero-card fade-up">

          <div class="hero-card-icon">
            ✦
          </div>

          <h3>
            One Business. Multiple Solutions.
          </h3>

          <p>
            A flexible service company focused on quality,
            convenience, and customer satisfaction.
          </p>

          <ul class="hero-list">
            <li>Professional & Reliable</li>
            <li>Customer-Focused Service</li>
            <li>Flexible Solutions</li>
            <li>Quality You Can Count On</li>
          </ul>

        </div>

      </div>

    </section>


    <!-- =========================
         SERVICES
    ========================= -->

    <section class="services" id="services">

      <div class="container">

        <div class="section-header">

          <div class="section-label">
            What We Do
          </div>

          <h2>
            Services For Every Need
          </h2>

          <p>
            We bring multiple services together under one trusted
            name, making it easier to get the help you need.
          </p>

        </div>


        <div class="services-grid">

          <div class="service-card">
            <div class="service-icon">🏠</div>
            <h3>Home Services</h3>
            <p>
              Convenient solutions designed to help keep your
              home comfortable, organized, and maintained.
            </p>
          </div>

          <div class="service-card">
            <div class="service-icon">💼</div>
            <h3>Business Services</h3>
            <p>
              Professional support and practical solutions
              designed for businesses of different sizes.
            </p>
          </div>

          <div class="service-card">
            <div class="service-icon">🧹</div>
            <h3>Cleaning Services</h3>
            <p>
              Reliable cleaning solutions for residential,
              commercial, and special-purpose spaces.
            </p>
          </div>

          <div class="service-card">
            <div class="service-icon">🔧</div>
            <h3>Maintenance</h3>
            <p>
              Dependable maintenance solutions that help
              protect and maintain your property.
            </p>
          </div>

          <div class="service-card">
            <div class="service-icon">🚚</div>
            <h3>Moving & Assistance</h3>
            <p>
              Helpful solutions for moving, transportation,
              organization, and everyday tasks.
            </p>
          </div>

          <div class="service-card">
            <div class="service-icon">✨</div>
            <h3>Custom Services</h3>
            <p>
              Have a unique request? Contact us to discuss
              a solution tailored specifically to your needs.
            </p>
          </div>

        </div>

      </div>

    </section>


    <!-- =========================
         ABOUT
    ========================= -->

    <section class="about" id="about">

      <div class="container about-grid">

        <div class="about-image">

          <div class="about-logo">
            <strong>YourDesire<span>Services</span></strong>
            <p>Solutions Made Simple</p>
          </div>

        </div>


        <div class="about-content">

          <div class="section-label">
            About Us
          </div>

          <h2>
            Built Around Your Needs
          </h2>

          <p>
            At YourDesireServices, our goal is simple:
            make professional services easier to access.
            We bring together practical solutions under
            one convenient business.
          </p>

          <p>
            We focus on communication, reliability,
            professionalism, and creating a positive
            experience for every customer.
          </p>

          <ul class="check-list">

            <li>
              <span>✓</span>
              Professional approach
            </li>

            <li>
              <span>✓</span>
              Flexible service options
            </li>

            <li>
              <span>✓</span>
              Customer-focused solutions
            </li>

            <li>
              <span>✓</span>
              Clear and convenient communication
            </li>

          </ul>

        </div>

      </div>

    </section>


    <!-- =========================
         WHY CHOOSE US
    ========================= -->

    <section>

      <div class="container">

        <div class="section-header">

          <div class="section-label">
            Why YourDesireServices
          </div>

          <h2>
            Service With Purpose
          </h2>

          <p>
            We believe good service starts with understanding
            what customers actually need.
          </p>

        </div>


        <div class="features-grid">

          <div class="feature">
            <div class="feature-number">01</div>
            <h3>Reliable</h3>
            <p>
              We value dependability and clear communication
              throughout every service.
            </p>
          </div>

          <div class="feature">
            <div class="feature-number">02</div>
            <h3>Professional</h3>
            <p>
              Every customer interaction is handled with
              respect and professionalism.
            </p>
          </div>

          <div class="feature">
            <div class="feature-number">03</div>
            <h3>Flexible</h3>
            <p>
              Our multi-purpose approach allows us to adapt
              services to different customer needs.
            </p>
          </div>

        </div>

      </div>

    </section>


    <!-- =========================
         CTA
    ========================= -->

    <section class="cta">

      <div class="container">

        <div class="cta-box">

          <div class="cta-content">

            <h2>
              Have Something In Mind?
            </h2>

            <p>
              Tell us what you need. Our team is ready to
              discuss your request and find a practical solution.
            </p>

            <a href="#contact" class="btn btn-primary">
              Request a Service
            </a>

          </div>

        </div>

      </div>

    </section>


    <!-- =========================
         CONTACT
    ========================= -->

    <section class="contact" id="contact">

      <div class="container contact-grid">

        <div class="contact-info">

          <div class="section-label">
            Contact Us
          </div>

          <h2>
            Let's Talk About Your Needs
          </h2>

          <p>
            Have questions or need a custom service?
            Send us a message and we'll get back to you.
          </p>


          <div class="contact-item">

            <div class="contact-item-icon">
              ✉
            </div>

            <div>
              <strong>Email</strong>
              <span>info@yourdesireservices.com</span>
            </div>

          </div>


          <div class="contact-item">

            <div class="contact-item-icon">
              ☎
            </div>

            <div>
              <strong>Phone</strong>
              <span>(555) 123-4567</span>
            </div>

          </div>


          <div class="contact-item">

            <div class="contact-item-icon">
              📍
            </div>

            <div>
              <strong>Service Area</strong>
              <span>Your City & Surrounding Areas</span>
            </div>

          </div>

        </div>


        <form class="contact-form" id="contactForm">

          <div class="form-group">

            <label for="name">
              Full Name
            </label>

            <input
              type="text"
              id="name"
              name="name"
              placeholder="Your name"
              required
            >

          </div>


          <div class="form-group">

            <label for="email">
              Email Address
            </label>

            <input
              type="email"
              id="email"
              name="email"
              placeholder="you@example.com"
              required
            >

          </div>


          <div class="form-group">

            <label for="service">
              Service Needed
            </label>

            <select id="service" name="service">

              <option value="">
                Select a service
              </option>

              <option value="home">
                Home Services
              </option>

              <option value="business">
                Business Services
              </option>

              <option value="cleaning">
                Cleaning Services
              </option>

              <option value="maintenance">
                Maintenance
              </option>

              <option value="moving">
                Moving & Assistance
              </option>

              <option value="custom">
                Custom Service
              </option>

            </select>

          </div>


          <div class="form-group">

            <label for="message">
              Message
            </label>

            <textarea
              id="message"
              name="message"
              placeholder="Tell us how we can help..."
              required
            ></textarea>

          </div>


          <button
            type="submit"
            class="btn btn-primary submit-btn"
          >
            Send Request
          </button>

        </form>

      </div>

    </section>

  </main>


  <!-- =========================
       FOOTER
  ========================= -->

  <footer>

    <div class="container">

      <div class="footer-grid">

        <div>

          <div class="footer-logo">
            YourDesire<span>Services</span>
          </div>

          <p class="footer-description">
            Professional multi-purpose services designed
            around your needs. Reliable solutions,
            convenient service, and customer-focused support.
          </p>

        </div>


        <div class="footer-column">

          <h4>Quick Links</h4>

          <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#services">Services</a></li>
            <li><a href="#about">About Us</a></li>
            <li><a href="#contact">Contact</a></li>
          </ul>

        </div>


        <div class="footer-column">

          <h4>Services</h4>

          <ul>
            <li><a href="#services">Home Services</a></li>
            <li><a href="#services">Business Services</a></li>
            <li><a href="#services">Cleaning</a></li>
            <li><a href="#services">Maintenance</a></li>
          </ul>

        </div>

      </div>


      <div class="footer-bottom">

        © <span id="year"></span> YourDesireServices.
        All rights reserved.

      </div>

    </div>

  </footer>


  <!-- =========================
       JAVASCRIPT
  ========================= -->

  <script>

    // Mobile navigation
    const menuToggle = document.getElementById("menuToggle");
    const navLinks = document.getElementById("navLinks");

    menuToggle.addEventListener("click", () => {
      navLinks.classList.toggle("active");
    });


    // Close mobile menu after clicking a link
    document.querySelectorAll(".nav-links a").forEach(link => {

      link.addEventListener("click", () => {
        navLinks.classList.remove("active");
      });

    });


    // Current year
    document.getElementById("year").textContent =
      new Date().getFullYear();


    // Contact form
    const contactForm = document.getElementById("contactForm");

    contactForm.addEventListener("submit", function(event) {

      event.preventDefault();

      const name = document.getElementById("name").value;

      alert(
        `Thank you, ${name}! Your request has been received.`
      );

      contactForm.reset();

    });

  </script>

</body>
</html>

