<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />

  <title>Bala Surfaces | Luxury Wall & Floor Tiles in Delhi</title>

  <meta
    name="description"
    content="Bala Surfaces offers premium wall tiles, floor tiles and luxury surface solutions in Delhi. Schedule a private consultation with our team."
  />

  <meta name="theme-color" content="#171512" />

  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

  <link
    href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;600;700&family=Playfair+Display:wght@400;500;600;700&display=swap"
    rel="stylesheet"
  />

  <style>
    :root {
      --black: #171512;
      --dark: #211e1a;
      --cream: #f4f0e8;
      --cream-light: #faf8f3;
      --gold: #b9975b;
      --gold-light: #d4b879;
      --text: #27231f;
      --muted: #756f67;
      --white: #ffffff;
      --border: rgba(23, 21, 18, 0.12);
      --shadow: 0 20px 60px rgba(23, 21, 18, 0.12);
      --radius: 2px;
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
      font-family: "DM Sans", sans-serif;
      color: var(--text);
      background: var(--cream-light);
      line-height: 1.6;
      overflow-x: hidden;
    }

    a {
      color: inherit;
      text-decoration: none;
    }

    button,
    input,
    select,
    textarea {
      font-family: inherit;
    }

    img {
      width: 100%;
      display: block;
      object-fit: cover;
    }

    .container {
      width: min(1180px, 92%);
      margin: auto;
    }

    /* =========================
       HEADER
    ========================= */

    header {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      z-index: 1000;
      transition: 0.3s ease;
      color: white;
    }

    header.scrolled {
      background: rgba(23, 21, 18, 0.96);
      backdrop-filter: blur(12px);
      box-shadow: 0 8px 30px rgba(0,0,0,0.12);
    }

    .nav {
      height: 82px;
      display: flex;
      align-items: center;
      justify-content: space-between;
    }

    .logo {
      display: flex;
      flex-direction: column;
      line-height: 1;
    }

    .logo-main {
      font-family: "Playfair Display", serif;
      font-size: 27px;
      letter-spacing: 1px;
    }

    .logo-sub {
      color: var(--gold-light);
      font-size: 9px;
      letter-spacing: 4px;
      margin-top: 7px;
      text-transform: uppercase;
    }

    .nav-links {
      display: flex;
      align-items: center;
      gap: 32px;
      list-style: none;
    }

    .nav-links a {
      font-size: 13px;
      letter-spacing: 0.5px;
      position: relative;
    }

    .nav-links a::after {
      content: "";
      position: absolute;
      left: 0;
      bottom: -7px;
      width: 0;
      height: 1px;
      background: var(--gold-light);
      transition: 0.3s;
    }

    .nav-links a:hover::after {
      width: 100%;
    }

    .nav-cta {
      border: 1px solid rgba(255,255,255,0.55);
      padding: 11px 18px;
      font-size: 12px;
      letter-spacing: 1px;
      text-transform: uppercase;
    }

    .menu-btn {
      display: none;
      background: none;
      border: 0;
      color: white;
      font-size: 28px;
      cursor: pointer;
    }

    /* =========================
       HERO
    ========================= */

    .hero {
      min-height: 100vh;
      position: relative;
      display: flex;
      align-items: center;
      color: white;
      background:
        linear-gradient(90deg, rgba(12,10,8,0.88), rgba(12,10,8,0.38)),
        url("https://images.unsplash.com/photo-1600607687939-ce8a6c25118c?auto=format&fit=crop&w=2000&q=90")
        center/cover;
    }

    .hero-content {
      max-width: 720px;
      padding-top: 90px;
    }

    .eyebrow {
      color: var(--gold-light);
      font-size: 11px;
      text-transform: uppercase;
      letter-spacing: 4px;
      margin-bottom: 20px;
      font-weight: 600;
    }

    .hero h1 {
      font-family: "Playfair Display", serif;
      font-weight: 500;
      font-size: clamp(48px, 7vw, 88px);
      line-height: 1.02;
      margin-bottom: 25px;
    }

    .hero h1 span {
      color: var(--gold-light);
    }

    .hero p {
      max-width: 570px;
      color: rgba(255,255,255,0.82);
      font-size: 17px;
      margin-bottom: 35px;
    }

    .hero-buttons {
      display: flex;
      flex-wrap: wrap;
      gap: 14px;
    }

    .btn {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      min-height: 50px;
      padding: 0 25px;
      border: 1px solid var(--gold);
      background: var(--gold);
      color: #171512;
      font-size: 12px;
      font-weight: 700;
      letter-spacing: 1.3px;
      text-transform: uppercase;
      cursor: pointer;
      transition: 0.3s;
    }

    .btn:hover {
      background: var(--gold-light);
      border-color: var(--gold-light);
      transform: translateY(-2px);
    }

    .btn-outline {
      background: transparent;
      color: white;
      border-color: rgba(255,255,255,0.55);
    }

    .btn-outline:hover {
      background: white;
      color: var(--black);
      border-color: white;
    }

    .hero-bottom {
      position: absolute;
      bottom: 35px;
      left: 0;
      width: 100%;
    }

    .hero-bottom-inner {
      display: flex;
      justify-content: space-between;
      align-items: center;
      color: rgba(255,255,255,0.65);
      font-size: 11px;
      letter-spacing: 2px;
      text-transform: uppercase;
    }

    /* =========================
       SECTION COMMON
    ========================= */

    section {
      padding: 105px 0;
    }

    .section-header {
      max-width: 700px;
      margin-bottom: 55px;
    }

    .section-header.center {
      margin-left: auto;
      margin-right: auto;
      text-align: center;
    }

    .section-title {
      font-family: "Playfair Display", serif;
      font-weight: 500;
      font-size: clamp(38px, 5vw, 60px);
      line-height: 1.1;
      margin-bottom: 20px;
    }

    .section-description {
      color: var(--muted);
      font-size: 16px;
    }

    .gold-line {
      width: 55px;
      height: 1px;
      background: var(--gold);
      margin: 20px 0;
    }

    .center .gold-line {
      margin-left: auto;
      margin-right: auto;
    }

    /* =========================
       INTRO
    ========================= */

    .intro {
      background: var(--cream-light);
    }

    .intro-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 90px;
      align-items: center;
    }

    .intro-image {
      height: 620px;
      background:
        url("https://images.unsplash.com/photo-1618221195710-dd6b41faaea6?auto=format&fit=crop&w=1200&q=85")
        center/cover;
    }

    .intro-text p {
      color: var(--muted);
      margin-bottom: 22px;
      font-size: 16px;
    }

    .signature {
      margin-top: 35px;
      font-family: "Playfair Display", serif;
      font-size: 24px;
    }

    /* =========================
       COLLECTIONS
    ========================= */

    .collections {
      background: var(--black);
      color: white;
    }

    .collections .section-description {
      color: rgba(255,255,255,0.62);
    }

    .collection-grid {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 15px;
    }

    .collection-card {
      height: 440px;
      position: relative;
      overflow: hidden;
      cursor: pointer;
    }

    .collection-card img {
      height: 100%;
      transition: transform 0.8s ease;
    }

    .collection-card:hover img {
      transform: scale(1.06);
    }

    .collection-overlay {
      position: absolute;
      inset: 0;
      display: flex;
      align-items: flex-end;
      padding: 28px;
      background: linear-gradient(transparent 40%, rgba(0,0,0,0.75));
    }

    .collection-overlay h3 {
      font-family: "Playfair Display", serif;
      font-size: 27px;
      font-weight: 500;
    }

    .collection-overlay span {
      display: block;
      color: var(--gold-light);
      font-size: 10px;
      text-transform: uppercase;
      letter-spacing: 2px;
      margin-top: 5px;
    }

    /* =========================
       PRODUCTS
    ========================= */

    .products {
      background: var(--cream);
    }

    .product-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 25px;
    }

    .product-card {
      background: white;
      overflow: hidden;
      box-shadow: 0 10px 35px rgba(0,0,0,0.06);
    }

    .product-image {
      height: 300px;
      overflow: hidden;
      position: relative;
    }

    .product-image img {
      height: 100%;
      transition: 0.6s;
    }

    .product-card:hover .product-image img {
      transform: scale(1.05);
    }

    .product-tag {
      position: absolute;
      top: 15px;
      left: 15px;
      background: var(--black);
      color: white;
      padding: 7px 11px;
      font-size: 9px;
      letter-spacing: 1.5px;
      text-transform: uppercase;
    }

    .product-content {
      padding: 24px;
    }

    .product-category {
      color: var(--gold);
      font-size: 9px;
      text-transform: uppercase;
      letter-spacing: 2px;
      font-weight: 700;
    }

    .product-content h3 {
      font-family: "Playfair Display", serif;
      font-size: 25px;
      margin: 7px 0;
      font-weight: 500;
    }

    .product-content p {
      color: var(--muted);
      font-size: 13px;
    }

    /* =========================
       STATS
    ========================= */

    .stats {
      background: var(--gold);
      padding: 55px 0;
    }

    .stats-grid {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      text-align: center;
    }

    .stat {
      padding: 10px 20px;
      border-right: 1px solid rgba(23,21,18,0.22);
    }

    .stat:last-child {
      border-right: none;
    }

    .stat strong {
      font-family: "Playfair Display", serif;
      font-size: 42px;
      font-weight: 500;
      display: block;
    }

    .stat span {
      font-size: 10px;
      letter-spacing: 2px;
      text-transform: uppercase;
    }

    /* =========================
       WHY US
    ========================= */

    .why-grid {
      display: grid;
      grid-template-columns: 0.9fr 1.1fr;
      gap: 90px;
      align-items: center;
    }

    .why-image {
      height: 650px;
      background:
        url("https://images.unsplash.com/photo-1600210492486-724fe5c67fb0?auto=format&fit=crop&w=1200&q=85")
        center/cover;
    }

    .features {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 35px 40px;
      margin-top: 40px;
    }

    .feature {
      border-top: 1px solid var(--border);
      padding-top: 20px;
    }

    .feature-number {
      color: var(--gold);
      font-size: 11px;
      letter-spacing: 2px;
    }

    .feature h3 {
      font-family: "Playfair Display", serif;
      font-size: 23px;
      font-weight: 500;
      margin: 7px 0;
    }

    .feature p {
      color: var(--muted);
      font-size: 13px;
    }

    /* =========================
       CTA
    ========================= */

    .cta {
      background:
        linear-gradient(rgba(20,17,14,0.86), rgba(20,17,14,0.86)),
        url("https://images.unsplash.com/photo-1600607687920-4e2a09cf159d?auto=format&fit=crop&w=2000&q=85")
        center/cover;
      color: white;
      text-align: center;
    }

    .cta .section-description {
      color: rgba(255,255,255,0.68);
      max-width: 620px;
      margin: auto;
    }

    .cta-buttons {
      display: flex;
      justify-content: center;
      gap: 15px;
      margin-top: 30px;
      flex-wrap: wrap;
    }

    /* =========================
       CONTACT
    ========================= */

    .contact {
      background: var(--cream);
    }

    .contact-grid {
      display: grid;
      grid-template-columns: 0.8fr 1.2fr;
      gap: 70px;
    }

    .contact-details {
      margin-top: 35px;
    }

    .contact-item {
      border-top: 1px solid var(--border);
      padding: 20px 0;
    }

    .contact-item span {
      display: block;
      color: var(--gold);
      font-size: 9px;
      letter-spacing: 2px;
      text-transform: uppercase;
      margin-bottom: 5px;
    }

    .contact-item a,
    .contact-item p {
      font-size: 16px;
    }

    .contact-form {
      background: white;
      padding: 40px;
      box-shadow: var(--shadow);
    }

    .form-title {
      font-family: "Playfair Display", serif;
      font-size: 32px;
      margin-bottom: 25px;
    }

    .form-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 18px;
    }

    .field {
      display: flex;
      flex-direction: column;
      gap: 7px;
    }

    .field.full {
      grid-column: 1 / -1;
    }

    label {
      font-size: 10px;
      letter-spacing: 1px;
      text-transform: uppercase;
      font-weight: 700;
    }

    input,
    select,
    textarea {
      width: 100%;
      border: 1px solid #ddd8cf;
      background: #faf9f6;
      padding: 14px;
      outline: none;
      color: var(--text);
      font-size: 14px;
      transition: 0.2s;
    }

    input:focus,
    select:focus,
    textarea:focus {
      border-color: var(--gold);
      background: white;
    }

    textarea {
      min-height: 120px;
      resize: vertical;
    }

    .form-submit {
      margin-top: 22px;
      width: 100%;
    }

    /* =========================
       FOOTER
    ========================= */

    footer {
      background: var(--black);
      color: white;
      padding: 65px 0 25px;
    }

    .footer-grid {
      display: grid;
      grid-template-columns: 1.4fr 1fr 1fr;
      gap: 70px;
      padding-bottom: 50px;
    }

    .footer-logo {
      font-family: "Playfair Display", serif;
      font-size: 34px;
    }

    footer p {
      color: rgba(255,255,255,0.55);
      font-size: 13px;
      max-width: 390px;
      margin-top: 15px;
    }

    .footer-heading {
      color: var(--gold-light);
      font-size: 10px;
      letter-spacing: 2px;
      text-transform: uppercase;
      margin-bottom: 18px;
    }

    .footer-links {
      list-style: none;
    }

    .footer-links li {
      margin: 9px 0;
      color: rgba(255,255,255,0.65);
      font-size: 13px;
    }

    .copyright {
      border-top: 1px solid rgba(255,255,255,0.1);
      padding-top: 22px;
      color: rgba(255,255,255,0.38);
      font-size: 11px;
      display: flex;
      justify-content: space-between;
    }

    /* =========================
       WHATSAPP
    ========================= */

    .whatsapp {
      position: fixed;
      right: 22px;
      bottom: 22px;
      width: 56px;
      height: 56px;
      border-radius: 50%;
      background: #25D366;
      color: white;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 25px;
      z-index: 900;
      box-shadow: 0 10px 30px rgba(0,0,0,0.2);
      transition: 0.3s;
    }

    .whatsapp:hover {
      transform: scale(1.08);
    }

    /* =========================
       MODAL
    ========================= */

    .modal {
      position: fixed;
      inset: 0;
      z-index: 2000;
      background: rgba(0,0,0,0.7);
      display: none;
      align-items: center;
      justify-content: center;
      padding: 20px;
      backdrop-filter: blur(5px);
    }

    .modal.active {
      display: flex;
    }

    .modal-box {
      width: min(700px, 100%);
      max-height: 90vh;
      overflow-y: auto;
      background: var(--cream-light);
      padding: 45px;
      position: relative;
      animation: modalIn 0.3s ease;
    }

    @keyframes modalIn {
      from {
        opacity: 0;
        transform: translateY(20px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    .modal-close {
      position: absolute;
      top: 18px;
      right: 20px;
      background: none;
      border: none;
      font-size: 28px;
      cursor: pointer;
      color: var(--muted);
    }

    .modal-box h2 {
      font-family: "Playfair Display", serif;
      font-size: 40px;
      font-weight: 500;
      margin-bottom: 8px;
    }

    .modal-intro {
      color: var(--muted);
      font-size: 14px;
      margin-bottom: 28px;
    }

    .meeting-step {
      display: none;
    }

    .meeting-step.active {
      display: block;
    }

    .step-title {
      font-size: 12px;
      letter-spacing: 1.5px;
      text-transform: uppercase;
      font-weight: 700;
      margin-bottom: 18px;
    }

    .time-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 10px;
      margin-top: 18px;
    }

    .time-btn {
      padding: 13px 8px;
      background: white;
      border: 1px solid #ddd8cf;
      cursor: pointer;
      transition: 0.2s;
      font-size: 13px;
    }

    .time-btn:hover,
    .time-btn.selected {
      background: var(--black);
      color: white;
      border-color: var(--black);
    }

    .selected-summary {
      background: #eee8dc;
      padding: 15px;
      margin: 20px 0;
      font-size: 13px;
    }

    .modal-actions {
      display: flex;
      justify-content: space-between;
      gap: 12px;
      margin-top: 25px;
    }

    .modal-actions .btn {
      flex: 1;
    }

    .success {
      text-align: center;
      padding: 30px 10px;
    }

    .success-icon {
      width: 65px;
      height: 65px;
      margin: 0 auto 20px;
      border-radius: 50%;
      background: var(--gold);
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 30px;
    }

    .success h3 {
      font-family: "Playfair Display", serif;
      font-size: 35px;
      margin-bottom: 10px;
    }

    .success p {
      color: var(--muted);
      font-size: 14px;
    }

    /* =========================
       MOBILE
    ========================= */

    @media (max-width: 900px) {
      .nav-links {
        position: absolute;
        top: 82px;
        left: 0;
        width: 100%;
        background: var(--black);
        padding: 25px;
        flex-direction: column;
        align-items: flex-start;
        display: none;
      }

      .nav-links.open {
        display: flex;
      }

      .menu-btn {
        display: block;
      }

      .nav-cta {
        display: none;
      }

      .collection-grid {
        grid-template-columns: 1fr 1fr;
      }

      .intro-grid,
      .why-grid,
      .contact-grid {
        grid-template-columns: 1fr;
        gap: 45px;
      }

      .intro-image,
      .why-image {
        height: 500px;
      }

      .product-grid {
        grid-template-columns: 1fr 1fr;
      }

      .stats-grid {
        grid-template-columns: 1fr 1fr;
        gap: 25px 0;
      }

      .stat:nth-child(2) {
        border-right: none;
      }

      .footer-grid {
        grid-template-columns: 1fr 1fr;
      }
    }

    @media (max-width: 600px) {
      section {
        padding: 75px 0;
      }

      .hero h1 {
        font-size: 48px;
      }

      .hero p {
        font-size: 15px;
      }

      .collection-grid,
      .product-grid,
      .features,
      .footer-grid,
      .form-grid {
        grid-template-columns: 1fr;
      }

      .collection-card {
        height: 380px;
      }

      .product-image {
        height: 280px;
      }

      .stats-grid {
        grid-template-columns: 1fr 1fr;
      }

      .stat {
        border-right: none;
        border-bottom: 1px solid rgba(23,21,18,0.18);
        padding-bottom: 20px;
      }

      .stat strong {
        font-size: 34px;
      }

      .contact-form {
        padding: 25px;
      }

      .modal-box {
        padding: 30px 20px;
      }

      .modal-box h2 {
        font-size: 32px;
      }

      .time-grid {
        grid-template-columns: 1fr 1fr;
      }

      .copyright {
        flex-direction: column;
        gap: 8px;
      }
    }
  </style>
</head>

<body>

  <!-- =========================
       HEADER
  ========================= -->

  <header id="header">
    <div class="container nav">

      <a href="#home" class="logo">
        <span class="logo-main">Bala Surfaces</span>
        <span class="logo-sub">Surfaces of Distinction</span>
      </a>

      <button class="menu-btn" id="menuBtn" aria-label="Open menu">
        ☰
      </button>

      <ul class="nav-links" id="navLinks">
        <li><a href="#home">Home</a></li>
        <li><a href="#collections">Collections</a></li>
        <li><a href="#products">Tiles</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>

      <button class="nav-cta" onclick="openMeetingModal()">
        Schedule Meeting
      </button>

    </div>
  </header>


  <!-- =========================
       HERO
  ========================= -->

  <main>

    <section class="hero" id="home">

      <div class="container">
        <div class="hero-content">

          <div class="eyebrow">
            Premium Surfaces • Delhi
          </div>

          <h1>
            Spaces Designed<br>
            with <span>Character.</span>
          </h1>

          <p>
            Discover refined wall tiles, floor tiles and premium surface
            collections curated for homes, hospitality and sophisticated
            commercial spaces.
          </p>

          <div class="hero-buttons">

            <a href="#collections" class="btn">
              Explore Collections
            </a>

            <button class="btn btn-outline" onclick="openMeetingModal()">
              Schedule a Consultation
            </button>

          </div>

        </div>
      </div>

      <div class="hero-bottom">
        <div class="container hero-bottom-inner">
          <span>Bala Surfaces</span>
          <span>Delhi • India</span>
        </div>
      </div>

    </section>


    <!-- =========================
         INTRO
    ========================= -->

    <section class="intro" id="about">

      <div class="container intro-grid">

        <div class="intro-image"></div>

        <div class="intro-text">

          <div class="eyebrow">
            The Bala Surfaces Philosophy
          </div>

          <h2 class="section-title">
            Beauty begins<br>
            beneath the surface.
          </h2>

          <div class="gold-line"></div>

          <p>
            At Bala Surfaces, we believe exceptional spaces begin with
            exceptional surfaces.
          </p>

          <p>
            Our collections bring together sophisticated textures,
            contemporary finishes and timeless materials to help architects,
            designers and homeowners create spaces that feel distinctly
            their own.
          </p>

          <p>
            From elegant wall tiles to statement flooring, every collection
            is selected with an eye for design, quality and enduring appeal.
          </p>

          <div class="signature">
            Bala Surfaces
          </div>

        </div>

      </div>

    </section>


    <!-- =========================
         COLLECTIONS
    ========================= -->

    <section class="collections" id="collections">

      <div class="container">

        <div class="section-header center">

          <div class="eyebrow">
            Explore Our World
          </div>

          <h2 class="section-title">
            Collections
          </h2>

          <div class="gold-line"></div>

          <p class="section-description">
            A curated selection of textures, patterns and finishes created
            to elevate contemporary interiors.
          </p>

        </div>


        <div class="collection-grid">

          <div class="collection-card">
            <img
              src="https://images.unsplash.com/photo-1615529162924-f8605388461d?auto=format&fit=crop&w=900&q=85"
              alt="Luxury marble surface"
            >

            <div class="collection-overlay">
              <div>
                <h3>Marble</h3>
                <span>Timeless elegance</span>
              </div>
            </div>
          </div>


          <div class="collection-card">
            <img
              src="https://images.unsplash.com/photo-1600566753190-17f0baa2a6c3?auto=format&fit=crop&w=900&q=85"
              alt="Stone surface"
            >

            <div class="collection-overlay">
              <div>
                <h3>Stone</h3>
                <span>Natural character</span>
              </div>
            </div>
          </div>


          <div class="collection-card">
            <img
              src="https://images.unsplash.com/photo-1600607688969-a5bfcd646154?auto=format&fit=crop&w=900&q=85"
              alt="Luxury wood surface"
            >

            <div class="collection-overlay">
              <div>
                <h3>Wood</h3>
                <span>Warm sophistication</span>
              </div>
            </div>
          </div>


          <div class="collection-card">
            <img
              src="https://images.unsplash.com/photo-1600607687920-4e2a09cf159d?auto=format&fit=crop&w=900&q=85"
              alt="Modern concrete interior"
            >

            <div class="collection-overlay">
              <div>
                <h3>Concrete</h3>
                <span>Modern minimalism</span>
              </div>
            </div>
          </div>

        </div>

      </div>

    </section>


    <!-- =========================
         PRODUCT COLLECTION
    ========================= -->

    <section class="products" id="products">

      <div class="container">

        <div class="section-header">

          <div class="eyebrow">
            Signature Selection
          </div>

          <h2 class="section-title">
            Surfaces for<br>every expression.
          </h2>

          <div class="gold-line"></div>

          <p class="section-description">
            Explore some of the styles available through our curated
            collection. Visit our showroom for the complete range.
          </p>

        </div>


        <div class="product-grid">

          <article class="product-card">

            <div class="product-image">
              <span class="product-tag">Wall Tile</span>

              <img
                src="https://images.unsplash.com/photo-1604709177225-055f99402ea3?auto=format&fit=crop&w=900&q=85"
                alt="Elegant neutral wall tile"
              >
            </div>

            <div class="product-content">
              <div class="product-category">
                Wall Collection
              </div>

              <h3>Ivory Vein</h3>

              <p>
                Soft neutral tones with delicate veining for sophisticated
                contemporary walls.
              </p>
            </div>

          </article>


          <article class="product-card">

            <div class="product-image">
              <span class="product-tag">Floor Tile</span>

              <img
                src="https://images.unsplash.com/photo-1600607687939-ce8a6c25118c?auto=format&fit=crop&w=900&q=85"
                alt="Luxury floor tile"
              >
            </div>

            <div class="product-content">
              <div class="product-category">
                Floor Collection
              </div>

              <h3>Stone Mist</h3>

              <p>
                A calm stone-inspired finish designed for elegant,
                expansive flooring.
              </p>
            </div>

          </article>


          <article class="product-card">

            <div class="product-image">
              <span class="product-tag">Premium</span>

              <img
                src="https://images.unsplash.com/photo-1618220179428-22790b461013?auto=format&fit=crop&w=900&q=85"
                alt="Luxury interior surface"
              >
            </div>

            <div class="product-content">
              <div class="product-category">
                Signature Collection
              </div>

              <h3>Travertine</h3>

              <p>
                Organic texture and warm tonal variation for timeless
                architectural interiors.
              </p>
            </div>

          </article>


          <article class="product-card">

            <div class="product-image">
              <span class="product-tag">Wall Tile</span>

              <img
                src="https://images.unsplash.com/photo-1617104678098-de229db51175?auto=format&fit=crop&w=900&q=85"
                alt="Decorative wall surface"
              >
            </div>

            <div class="product-content">
              <div class="product-category">
                Designer Collection
              </div>

              <h3>Calacatta</h3>

              <p>
                Dramatic veining and luxurious tones for statement walls
                and feature areas.
              </p>
            </div>

          </article>


          <article class="product-card">

            <div class="product-image">
              <span class="product-tag">Floor Tile</span>

              <img
                src="https://images.unsplash.com/photo-1600210491892-03d54c0aaf87?auto=format&fit=crop&w=900&q=85"
                alt="Premium flooring"
              >
            </div>

            <div class="product-content">
              <div class="product-category">
                Contemporary Floor
              </div>

              <h3>Graphite Stone</h3>

              <p>
                Deep sophisticated tones for bold modern architecture.
              </p>
            </div>

          </article>


          <article class="product-card">

            <div class="product-image">
              <span class="product-tag">Luxury</span>

              <img
                src="https://images.unsplash.com/photo-1615529328331-f8917597711f?auto=format&fit=crop&w=900&q=85"
                alt="Premium marble tile"
              >
            </div>

            <div class="product-content">
              <div class="product-category">
                Marble Collection
              </div>

              <h3>Arabescato</h3>

              <p>
                Expressive natural movement with a refined architectural
                finish.
              </p>
            </div>

          </article>

        </div>

      </div>

    </section>


    <!-- =========================
         STATS
    ========================= -->

    <section class="stats">

      <div class="container stats-grid">

        <div class="stat">
          <strong>01</strong>
          <span>Curated Design</span>
        </div>

        <div class="stat">
          <strong>02</strong>
          <span>Premium Surfaces</span>
        </div>

        <div class="stat">
          <strong>03</strong>
          <span>Design Guidance</span>
        </div>

        <div class="stat">
          <strong>04</strong>
          <span>Personal Service</span>
        </div>

      </div>

    </section>


    <!-- =========================
         WHY BALA SURFACES
    ========================= -->

    <section>

      <div class="container why-grid">

        <div class="why-image"></div>

        <div>

          <div class="eyebrow">
            Why Bala Surfaces
          </div>

          <h2 class="section-title">
            More than tiles.<br>
            A design experience.
          </h2>

          <div class="gold-line"></div>

          <p class="section-description">
            Choosing a surface is about more than colour and texture.
            It is about understanding how a material will transform the
            entire atmosphere of a space.
          </p>


          <div class="features">

            <div class="feature">
              <div class="feature-number">01</div>
              <h3>Curated Range</h3>
              <p>
                Carefully selected designs for modern and timeless spaces.
              </p>
            </div>

            <div class="feature">
              <div class="feature-number">02</div>
              <h3>Personal Guidance</h3>
              <p>
                Our team helps you find surfaces suited to your project.
              </p>
            </div>

            <div class="feature">
              <div class="feature-number">03</div>
              <h3>Premium Finishes</h3>
              <p>
                Explore refined textures, tones and contemporary finishes.
              </p>
            </div>

            <div class="feature">
              <div class="feature-number">04</div>
              <h3>Private Consultation</h3>
              <p>
                Schedule a dedicated meeting with our team at your
                convenience.
              </p>
            </div>

          </div>

        </div>

      </div>

    </section>


    <!-- =========================
         CTA
    ========================= -->

    <section class="cta">

      <div class="container">

        <div class="eyebrow">
          Your Space. Your Expression.
        </div>

        <h2 class="section-title">
          Let's create something<br>
          extraordinary.
        </h2>

        <p class="section-description">
          Visit Bala Surfaces or schedule a private consultation with our
          team to discuss your project.
        </p>

        <div class="cta-buttons">

          <button class="btn" onclick="openMeetingModal()">
            Schedule a Meeting
          </button>

          <a
            class="btn btn-outline"
            href="tel:+919650285586"
          >
            Call 9650285586
          </a>

        </div>

      </div>

    </section>


    <!-- =========================
         CONTACT
    ========================= -->

    <section class="contact" id="contact">

      <div class="container contact-grid">

        <div>

          <div class="eyebrow">
            Visit / Contact
          </div>

          <h2 class="section-title">
            Let's talk<br>
            about your space.
          </h2>

          <div class="gold-line"></div>

          <p class="section-description">
            Tell us about your project and our team will get in touch with
            you.
          </p>


          <div class="contact-details">

            <div class="contact-item">
              <span>Phone</span>
              <a href="tel:+919650285586">
                +91 96502 85586
              </a>
            </div>

            <div class="contact-item">
              <span>Email</span>
              <a href="mailto:balasurfaces26@gmail.com">
                balasurfaces26@gmail.com
              </a>
            </div>

            <div class="contact-item">
              <span>Location</span>
              <p>Delhi, India</p>
            </div>

            <div class="contact-item">
              <span>Appointments</span>
              <p>Private consultations available</p>
            </div>

          </div>

        </div>


        <div class="contact-form">

          <h3 class="form-title">
            Send an enquiry
          </h3>

          <form
            id="contactForm"
            action="YOUR_FORMSPREE_ENDPOINT"
            method="POST"
          >

            <div class="form-grid">

              <div class="field">
                <label for="name">Full Name</label>
                <input
                  type="text"
                  id="name"
                  name="name"
                  placeholder="Your full name"
                  required
                >
              </div>

              <div class="field">
                <label for="phone">Contact Number</label>
                <input
                  type="tel"
                  id="phone"
                  name="phone"
                  placeholder="+91"
                  required
                >
              </div>

              <div class="field">
                <label for="email">Email Address</label>
                <input
                  type="email"
                  id="email"
                  name="email"
                  placeholder="you@example.com"
                  required
                >
              </div>

              <div class="field">
                <label for="project">Project Type</label>

                <select id="project" name="project">
                  <option value="Residential">Residential</option>
                  <option value="Commercial">Commercial</option>
                  <option value="Hospitality">Hospitality</option>
                  <option value="Architect / Designer">
                    Architect / Designer
                  </option>
                  <option value="Other">Other</option>
                </select>

              </div>

              <div class="field full">

                <label for="message">
                  Tell us about your project
                </label>

                <textarea
                  id="message"
                  name="message"
                  placeholder="Tell us what you are looking for..."
                ></textarea>

              </div>

            </div>

            <button type="submit" class="btn form-submit">
              Send Enquiry
            </button>

          </form>

        </div>

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
            Bala Surfaces
          </div>

          <p>
            Premium wall tiles, floor tiles and surface solutions for
            refined spaces in Delhi.
          </p>

        </div>


        <div>

          <div class="footer-heading">
            Explore
          </div>

          <ul class="footer-links">
            <li><a href="#home">Home</a></li>
            <li><a href="#collections">Collections</a></li>
            <li><a href="#products">Tiles</a></li>
            <li><a href="#about">About</a></li>
          </ul>

        </div>


        <div>

          <div class="footer-heading">
            Contact
          </div>

          <ul class="footer-links">
            <li>Delhi, India</li>
            <li>
              <a href="tel:+919650285586">
                +91 96502 85586
              </a>
            </li>
            <li>
              <a href="mailto:balasurfaces26@gmail.com">
                balasurfaces26@gmail.com
              </a>
            </li>
          </ul>

        </div>

      </div>


      <div class="copyright">

        <span>
          © <span id="year"></span> Bala Surfaces. All rights reserved.
        </span>

        <span>
          Surfaces of Distinction
        </span>

      </div>

    </div>

  </footer>


  <!-- =========================
       WHATSAPP
  ========================= -->

  <a
    class="whatsapp"
    href="https://wa.me/919650285586?text=Hello%20Bala%20Surfaces,%20I%20would%20like%20to%20know%20more%20about%20your%20tiles%20and%20surfaces."
    target="_blank"
    aria-label="Contact Bala Surfaces on WhatsApp"
  >
    ☎
  </a>


  <!-- =========================
       MEETING MODAL
  ========================= -->

  <div class="modal" id="meetingModal">

    <div class="modal-box">

      <button
        class="modal-close"
        onclick="closeMeetingModal()"
        aria-label="Close"
      >
        ×
      </button>


      <div id="meetingStep1" class="meeting-step active">

        <div class="eyebrow">
          Private Consultation
        </div>

        <h2>Schedule a meeting</h2>

        <p class="modal-intro">
          Select your preferred date and time. On the next step,
          we'll collect your contact details so our team can confirm
          your appointment.
        </p>


        <div class="field">

          <label for="meetingDate">
            Select Date
          </label>

          <input
            type="date"
            id="meetingDate"
            required
          >

        </div>


        <div style="margin-top:25px;">

          <div class="step-title">
            Select Time
          </div>

          <div class="time-grid">

            <button class="time-btn" data-time="10:00 AM">
              10:00 AM
            </button>

            <button class="time-btn" data-time="11:00 AM">
              11:00 AM
            </button>

            <button class="time-btn" data-time="12:00 PM">
              12:00 PM
            </button>

            <button class="time-btn" data-time="02:00 PM">
              02:00 PM
            </button>

            <button class="time-btn" data-time="03:00 PM">
              03:00 PM
            </button>

            <button class="time-btn" data-time="04:00 PM">
              04:00 PM
            </button>

            <button class="time-btn" data-time="05:00 PM">
              05:00 PM
            </button>

            <button class="time-btn" data-time="06:00 PM">
              06:00 PM
            </button>

          </div>

        </div>


        <div class="modal-actions">

          <button
            class="btn"
            onclick="goToCustomerDetails()"
          >
            Continue
          </button>

        </div>

      </div>


      <!-- STEP 2 -->

      <div id="meetingStep2" class="meeting-step">

        <div class="eyebrow">
          Your Details
        </div>

        <h2>Tell us about you</h2>

        <p class="modal-intro">
          Please provide your details so our team can contact you and
          confirm your meeting.
        </p>


        <div class="selected-summary" id="selectedSummary">
          Your selected appointment will appear here.
        </div>


        <form id="meetingForm">

          <div class="form-grid">

            <div class="field">
              <label for="meetingName">
                Full Name
              </label>

              <input
                type="text"
                id="meetingName"
                name="full_name"
                placeholder="Your full name"
                required
              >
            </div>


            <div class="field">
              <label for="meetingPhone">
                Contact Number
              </label>

              <input
                type="tel"
                id="meetingPhone"
                name="contact_number"
                placeholder="+91"
                required
              >
            </div>


            <div class="field">
              <label for="meetingEmail">
                Email Address
              </label>

              <input
                type="email"
                id="meetingEmail"
                name="email"
                placeholder="you@example.com"
                required
              >
            </div>


            <div class="field">
              <label for="meetingCity">
                City
              </label>

              <input
                type="text"
                id="meetingCity"
                name="city"
                placeholder="Delhi"
                value="Delhi"
              >
            </div>


            <div class="field">
              <label for="meetingProject">
                Project Type
              </label>

              <select
                id="meetingProject"
                name="project_type"
              >
                <option value="Residential">
                  Residential
                </option>

                <option value="Commercial">
                  Commercial
                </option>

                <option value="Hospitality">
                  Hospitality
                </option>

                <option value="Architect / Designer">
                  Architect / Designer
                </option>

                <option value="Other">
                  Other
                </option>
              </select>

            </div>


            <div class="field">
              <label for="meetingArea">
                Approx. Project Size
              </label>

              <select
                id="meetingArea"
                name="project_size"
              >
                <option value="Not decided">
                  Not decided
                </option>

                <option value="Under 500 sq.ft">
                  Under 500 sq.ft
                </option>

                <option value="500 - 1500 sq.ft">
                  500 - 1500 sq.ft
                </option>

                <option value="1500 - 3000 sq.ft">
                  1500 - 3000 sq.ft
                </option>

                <option value="3000+ sq.ft">
                  3000+ sq.ft
                </option>
              </select>

            </div>


            <div class="field full">

              <label for="meetingMessage">
                Anything else you'd like us to know?
              </label>

              <textarea
                id="meetingMessage"
                name="message"
                placeholder="Tell us about your project, preferred tile style, requirements, etc."
              ></textarea>

            </div>

          </div>


          <input
            type="hidden"
            name="appointment_date"
            id="hiddenDate"
          >

          <input
            type="hidden"
            name="appointment_time"
            id="hiddenTime"
          >


          <div class="modal-actions">

            <button
              type="button"
              class="btn btn-outline"
              onclick="backToDateSelection()"
              style="color:#171512;border-color:#999;"
            >
              Back
            </button>

            <button
              type="submit"
              class="btn"
            >
              Request Meeting
            </button>

          </div>

        </form>

      </div>


      <!-- SUCCESS -->

      <div id="meetingSuccess" class="meeting-step">

        <div class="success">

          <div class="success-icon">
            ✓
          </div>

          <h3>Request received.</h3>

          <p>
            Thank you for choosing Bala Surfaces.
            Our team will contact you shortly to confirm your meeting.
          </p>

          <div
            class="selected-summary"
            id="successSummary"
            style="margin-top:25px;"
          ></div>

          <button
            class="btn"
            onclick="closeMeetingModal()"
          >
            Done
          </button>

        </div>

      </div>

    </div>

  </div>


  <!-- =========================
       JAVASCRIPT
  ========================= -->

  <script>

    /* =========================
       BASIC UI
    ========================= */

    const header = document.getElementById("header");

    window.addEventListener("scroll", () => {

      if (window.scrollY > 40) {
        header.classList.add("scrolled");
      } else {
        header.classList.remove("scrolled");
      }

    });


    const menuBtn = document.getElementById("menuBtn");
    const navLinks = document.getElementById("navLinks");

    menuBtn.addEventListener("click", () => {
      navLinks.classList.toggle("open");
    });


    document.querySelectorAll(".nav-links a").forEach(link => {

      link.addEventListener("click", () => {
        navLinks.classList.remove("open");
      });

    });


    document.getElementById("year").textContent =
      new Date().getFullYear();


    /* =========================
       MEETING SYSTEM
    ========================= */

    const modal = document.getElementById("meetingModal");

    const meetingDate =
      document.getElementById("meetingDate");

    let selectedTime = "";

    const today = new Date();

    const yyyy = today.getFullYear();

    const mm = String(today.getMonth() + 1).padStart(2, "0");

    const dd = String(today.getDate()).padStart(2, "0");

    meetingDate.min = `${yyyy}-${mm}-${dd}`;


    function openMeetingModal() {

      modal.classList.add("active");

      document.body.style.overflow = "hidden";

      showStep("meetingStep1");

    }


    function closeMeetingModal() {

      modal.classList.remove("active");

      document.body.style.overflow = "";

    }


    modal.addEventListener("click", (event) => {

      if (event.target === modal) {
        closeMeetingModal();
      }

    });


    document.querySelectorAll(".time-btn").forEach(button => {

      button.addEventListener("click", () => {

        document
          .querySelectorAll(".time-btn")
          .forEach(btn => btn.classList.remove("selected"));

        button.classList.add("selected");

        selectedTime = button.dataset.time;

      });

    });


    function showStep(stepId) {

      document
        .querySelectorAll(".meeting-step")
        .forEach(step => {
          step.classList.remove("active");
        });

      document
        .getElementById(stepId)
        .classList.add("active");

    }


    function formatDate(dateString) {

      const date = new Date(dateString + "T00:00:00");

      return date.toLocaleDateString("en-IN", {
        weekday: "long",
        day: "numeric",
        month: "long",
        year: "numeric"
      });

    }


    function goToCustomerDetails() {

      if (!meetingDate.value) {
        alert("Please select a date.");
        return;
      }

      if (!selectedTime) {
        alert("Please select a preferred time.");
        return;
      }

      const readableDate =
        formatDate(meetingDate.value);

      document.getElementById("selectedSummary").innerHTML =
        `<strong>Preferred appointment</strong><br>
         ${readableDate} at ${selectedTime}`;

      document.getElementById("hiddenDate").value =
        readableDate;

      document.getElementById("hiddenTime").value =
        selectedTime;

      showStep("meetingStep2");

    }


    function backToDateSelection() {

      showStep("meetingStep1");

    }


    /* =========================
       MEETING FORM
    ========================= */

    document
      .getElementById("meetingForm")
      .addEventListener("submit", async function(event) {

        event.preventDefault();

        const name =
          document.getElementById("meetingName").value;

        const phone =
          document.getElementById("meetingPhone").value;

        const email =
          document.getElementById("meetingEmail").value;

        const city =
          document.getElementById("meetingCity").value;

        const project =
          document.getElementById("meetingProject").value;

        const area =
          document.getElementById("meetingArea").value;

        const message =
          document.getElementById("meetingMessage").value;


        /*
          IMPORTANT:

          Replace the WhatsApp message below with your preferred
          business workflow if needed.
        */

        const whatsappMessage =
          `Hello Bala Surfaces,

I would like to request a consultation.

Name: ${name}
Phone: ${phone}
Email: ${email}
City: ${city}
Project: ${project}
Project Size: ${area}

Preferred Date: ${formatDate(meetingDate.value)}
Preferred Time: ${selectedTime}

Message:
${message || "No additional message."}

Please contact me to confirm the meeting.`;


        /*
          Open WhatsApp for the customer/team.

          This gives you an immediate notification even before
          connecting a backend form service.
        */

        const whatsappURL =
          "https://wa.me/919650285586?text=" +
          encodeURIComponent(whatsappMessage);


        /*
          Open WhatsApp in a new tab.
        */

        window.open(whatsappURL, "_blank");


        /*
          Show success screen.
        */

        document.getElementById("successSummary").innerHTML =
          `<strong>${formatDate(meetingDate.value)}</strong><br>
           Preferred time: ${selectedTime}<br><br>
           Our team will contact you on ${phone}.`;

        showStep("meetingSuccess");

      });


    /* =========================
       CONTACT FORM
    ========================= */

    document
      .getElementById("contactForm")
      .addEventListener("submit", function(event) {

        const formAction = this.getAttribute("action");

        if (
          !formAction ||
          formAction === "YOUR_FORMSPREE_ENDPOINT"
        ) {

          event.preventDefault();

          alert(
            "The enquiry form needs to be connected to your form service before it can receive submissions. Please follow the setup instructions below."
          );

        }

      });


    /* =========================
       ESCAPE KEY
    ========================= */

    document.addEventListener("keydown", event => {

      if (event.key === "Escape") {
        closeMeetingModal();
      }

    });

  </script>

</body>
</html>

.






