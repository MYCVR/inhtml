<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>Bala Surfaces | Premium Tiles in Delhi</title>

  <meta
    name="description"
    content="Bala Surfaces - Premium wall tiles, floor tiles and surfaces in Delhi."
  >

  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

  <link
    href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;600;700&family=Playfair+Display:wght@500;600&display=swap"
    rel="stylesheet"
  >

  <style>

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
      color: #222;
      background: #f8f6f1;
      line-height: 1.6;
    }

    a {
      text-decoration: none;
      color: inherit;
    }

    button,
    input,
    select,
    textarea {
      font-family: inherit;
    }

    .container {
      width: 90%;
      max-width: 1100px;
      margin: auto;
    }

    /* =========================
       HEADER
    ========================= */

    header {
      background: #151515;
      color: white;
      position: sticky;
      top: 0;
      z-index: 1000;
    }

    .navbar {
      height: 75px;
      display: flex;
      align-items: center;
      justify-content: space-between;
    }

    .logo {
      font-family: "Playfair Display", serif;
      font-size: 27px;
      color: #d6b36a;
    }

    nav {
      display: flex;
      gap: 28px;
    }

    nav a {
      font-size: 14px;
      color: #eee;
      transition: 0.3s;
    }

    nav a:hover {
      color: #d6b36a;
    }

    .header-button {
      background: #d6b36a;
      color: #151515;
      padding: 11px 18px;
      border: none;
      cursor: pointer;
      font-weight: 600;
      border-radius: 2px;
    }

    /* =========================
       HERO
    ========================= */

    .hero {
      min-height: 620px;

      background:
        linear-gradient(
          rgba(0,0,0,0.55),
          rgba(0,0,0,0.55)
        ),
        url("https://images.unsplash.com/photo-1600607687920-4e2a09cf159d?auto=format&fit=crop&w=1800&q=85");

      background-size: cover;
      background-position: center;

      display: flex;
      align-items: center;

      color: white;
    }

    .hero-content {
      max-width: 650px;
    }

    .hero-small {
      color: #d6b36a;
      text-transform: uppercase;
      letter-spacing: 3px;
      font-size: 12px;
      margin-bottom: 18px;
    }

    .hero h1 {
      font-family: "Playfair Display", serif;
      font-size: clamp(48px, 7vw, 75px);
      line-height: 1.05;
      font-weight: 500;
      margin-bottom: 20px;
    }

    .hero h1 span {
      color: #d6b36a;
    }

    .hero p {
      max-width: 570px;
      color: #ddd;
      font-size: 17px;
      margin-bottom: 30px;
    }

    .button {
      display: inline-block;
      background: #d6b36a;
      color: #151515;
      padding: 14px 24px;
      border: none;
      cursor: pointer;
      font-weight: 700;
      font-size: 13px;
      letter-spacing: 0.5px;
      border-radius: 2px;
    }

    .button:hover {
      background: #e5c681;
    }

    .button-outline {
      margin-left: 10px;
      background: transparent;
      border: 1px solid white;
      color: white;
    }

    .button-outline:hover {
      background: white;
      color: #151515;
    }

    /* =========================
       SECTIONS
    ========================= */

    section {
      padding: 80px 0;
    }

    .section-title {
      font-family: "Playfair Display", serif;
      font-size: 45px;
      font-weight: 500;
      margin-bottom: 15px;
    }

    .section-subtitle {
      color: #777;
      max-width: 600px;
      margin-bottom: 45px;
    }

    .gold-line {
      width: 50px;
      height: 2px;
      background: #d6b36a;
      margin: 15px 0 25px;
    }

    /* =========================
       ABOUT
    ========================= */

    .about {
      background: #f8f6f1;
    }

    .about-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 60px;
      align-items: center;
    }

    .about-image {
      height: 500px;

      background:
        url("https://images.unsplash.com/photo-1618221195710-dd6b41faaea6?auto=format&fit=crop&w=1000&q=85");

      background-size: cover;
      background-position: center;
    }

    .about-text p {
      color: #666;
      margin-bottom: 18px;
    }

    /* =========================
       COLLECTIONS
    ========================= */

    .collections {
      background: #181818;
      color: white;
    }

    .collections .section-subtitle {
      color: #aaa;
    }

    .collection-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 20px;
    }

    .collection {
      height: 300px;
      position: relative;
      overflow: hidden;
    }

    .collection img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      transition: 0.5s;
    }

    .collection:hover img {
      transform: scale(1.06);
    }

    .collection-text {
      position: absolute;
      left: 0;
      right: 0;
      bottom: 0;

      padding: 25px;

      background:
        linear-gradient(
          transparent,
          rgba(0,0,0,0.8)
        );
    }

    .collection-text h3 {
      font-family: "Playfair Display", serif;
      font-size: 27px;
    }

    /* =========================
       PRODUCTS
    ========================= */

    .products {
      background: #eeeae2;
    }

    .product-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 22px;
    }

    .product {
      background: white;
      padding-bottom: 20px;
    }

    .product img {
      width: 100%;
      height: 230px;
      object-fit: cover;
    }

    .product-content {
      padding: 20px;
    }

    .product-category {
      color: #b08b43;
      font-size: 11px;
      text-transform: uppercase;
      letter-spacing: 1px;
      font-weight: 700;
    }

    .product h3 {
      font-family: "Playfair Display", serif;
      font-size: 24px;
      margin: 6px 0;
    }

    .product p {
      color: #777;
      font-size: 13px;
    }

    /* =========================
       MEETING
    ========================= */

    .meeting {
      background: #151515;
      color: white;
    }

    .meeting-wrapper {
      max-width: 850px;
      margin: auto;
      text-align: center;
    }

    .meeting .section-subtitle {
      color: #aaa;
      margin-left: auto;
      margin-right: auto;
    }

    .meeting-box {
      background: white;
      color: #222;
      padding: 40px;
      text-align: left;
      margin-top: 35px;
    }

    .meeting-box h3 {
      font-family: "Playfair Display", serif;
      font-size: 30px;
      margin-bottom: 25px;
    }

    .form-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 18px;
    }

    .form-group {
      display: flex;
      flex-direction: column;
      gap: 7px;
    }

    .form-group.full {
      grid-column: 1 / -1;
    }

    label {
      font-size: 12px;
      font-weight: 600;
    }

    input,
    select,
    textarea {
      border: 1px solid #ddd;
      padding: 13px;
      font-size: 14px;
      outline: none;
      background: #fafafa;
    }

    input:focus,
    select:focus,
    textarea:focus {
      border-color: #c29e5a;
    }

    textarea {
      min-height: 100px;
      resize: vertical;
    }

    .submit-button {
      margin-top: 20px;
      width: 100%;
      border: none;
      background: #151515;
      color: white;
      padding: 15px;
      cursor: pointer;
      font-weight: 700;
    }

    .submit-button:hover {
      background: #d6b36a;
      color: #151515;
    }

    .notice {
      margin-top: 15px;
      color: #777;
      font-size: 12px;
      text-align: center;
    }

    /* =========================
       CONTACT
    ========================= */

    .contact {
      background: #f8f6f1;
    }

    .contact-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 60px;
    }

    .contact-item {
      padding: 20px 0;
      border-bottom: 1px solid #ddd;
    }

    .contact-item strong {
      display: block;
      color: #b08b43;
      font-size: 11px;
      text-transform: uppercase;
      letter-spacing: 1px;
      margin-bottom: 5px;
    }

    .contact-item a:hover {
      color: #b08b43;
    }

    /* =========================
       FOOTER
    ========================= */

    footer {
      background: #151515;
      color: white;
      text-align: center;
      padding: 35px 20px;
    }

    footer .footer-logo {
      font-family: "Playfair Display", serif;
      font-size: 28px;
      color: #d6b36a;
      margin-bottom: 10px;
    }

    footer p {
      color: #888;
      font-size: 13px;
    }

    /* =========================
       WHATSAPP
    ========================= */

    .whatsapp {
      position: fixed;
      right: 20px;
      bottom: 20px;

      width: 55px;
      height: 55px;

      background: #25D366;
      color: white;

      border-radius: 50%;

      display: flex;
      align-items: center;
      justify-content: center;

      font-size: 24px;

      z-index: 1000;

      box-shadow: 0 5px 20px rgba(0,0,0,0.25);
    }

    /* =========================
       MOBILE
    ========================= */

    @media (max-width: 800px) {

      nav {
        display: none;
      }

      .header-button {
        padding: 9px 12px;
        font-size: 11px;
      }

      .hero {
        min-height: 570px;
      }

      .hero h1 {
        font-size: 48px;
      }

      .about-grid,
      .contact-grid {
        grid-template-columns: 1fr;
      }

      .collection-grid,
      .product-grid {
        grid-template-columns: 1fr;
      }

      .about-image {
        height: 350px;
      }

      .form-grid {
        grid-template-columns: 1fr;
      }

      .form-group.full {
        grid-column: auto;
      }

      .meeting-box {
        padding: 25px;
      }

      .button-outline {
        margin-left: 0;
        margin-top: 10px;
      }

    }

  </style>
</head>

<body>

  <!-- HEADER -->

  <header>

    <div class="container navbar">

      <div class="logo">
        Bala Surfaces
      </div>

      <nav>
        <a href="#home">Home</a>
        <a href="#about">About</a>
        <a href="#collections">Collections</a>
        <a href="#products">Tiles</a>
        <a href="#meeting">Meeting</a>
        <a href="#contact">Contact</a>
      </nav>

      <a href="#meeting" class="header-button">
        Schedule Meeting
      </a>

    </div>

  </header>


  <!-- HERO -->

  <section class="hero" id="home">

    <div class="container">

      <div class="hero-content">

        <div class="hero-small">
          Premium Surfaces • Delhi
        </div>

        <h1>
          Beautiful surfaces.<br>
          <span>Beautiful spaces.</span>
        </h1>

        <p>
          Discover premium wall tiles, floor tiles and elegant surface
          solutions designed to transform your home or commercial space.
        </p>

        <a href="#collections" class="button">
          Explore Collections
        </a>

        <a href="#meeting" class="button button-outline">
          Schedule Meeting
        </a>

      </div>

    </div>

  </section>


  <!-- ABOUT -->

  <section class="about" id="about">

    <div class="container about-grid">

      <div class="about-image"></div>

      <div class="about-text">

        <div class="hero-small">
          About Bala Surfaces
        </div>

        <h2 class="section-title">
          Surfaces that define spaces.
        </h2>

        <div class="gold-line"></div>

        <p>
          Bala Surfaces brings together premium wall tiles, floor tiles
          and surface solutions for customers looking for quality,
          elegance and contemporary design.
        </p>

        <p>
          Whether you are designing a new home, renovating an existing
          property or working on a commercial project, our team can help
          you discover the right surface for your space.
        </p>

        <p>
          Visit us in Delhi or schedule a consultation with our team.
        </p>

      </div>

    </div>

  </section>


  <!-- COLLECTIONS -->

  <section class="collections" id="collections">

    <div class="container">

      <div class="hero-small">
        Our Collections
      </div>

      <h2 class="section-title">
        Explore our surfaces.
      </h2>

      <div class="gold-line"></div>

      <p class="section-subtitle">
        A selection of elegant materials and finishes for modern
        interiors.
      </p>


      <div class="collection-grid">

        <div class="collection">

          <img
            src="https://images.unsplash.com/photo-1615529162924-f8605388461d?auto=format&fit=crop&w=900&q=80"
            alt="Marble"
          >

          <div class="collection-text">
            <h3>Marble</h3>
            <p>Timeless luxury</p>
          </div>

        </div>


        <div class="collection">

          <img
            src="https://images.unsplash.com/photo-1600566753190-17f0baa2a6c3?auto=format&fit=crop&w=900&q=80"
            alt="Stone"
          >

          <div class="collection-text">
            <h3>Stone</h3>
            <p>Natural character</p>
          </div>

        </div>


        <div class="collection">

          <img
            src="https://images.unsplash.com/photo-1600607688969-a5bfcd646154?auto=format&fit=crop&w=900&q=80"
            alt="Wood"
          >

          <div class="collection-text">
            <h3>Wood</h3>
            <p>Warm elegance</p>
          </div>

        </div>

      </div>

    </div>

  </section>


  <!-- PRODUCTS -->

  <section class="products" id="products">

    <div class="container">

      <div class="hero-small">
        Featured Tiles
      </div>

      <h2 class="section-title">
        Designed for every space.
      </h2>

      <div class="gold-line"></div>

      <p class="section-subtitle">
        Explore a few of our featured styles. Contact our team for
        the complete collection.
      </p>


      <div class="product-grid">

        <div class="product">

          <img
            src="https://images.unsplash.com/photo-1604709177225-055f99402ea3?auto=format&fit=crop&w=900&q=80"
            alt="Wall tile"
          >

          <div class="product-content">

            <div class="product-category">
              Wall Tile
            </div>

            <h3>Ivory Vein</h3>

            <p>
              Elegant neutral tones for sophisticated interiors.
            </p>

          </div>

        </div>


        <div class="product">

          <img
            src="https://images.unsplash.com/photo-1600607687939-ce8a6c25118c?auto=format&fit=crop&w=900&q=80"
            alt="Floor tile"
          >

          <div class="product-content">

            <div class="product-category">
              Floor Tile
            </div>

            <h3>Stone Mist</h3>

            <p>
              A refined stone-inspired finish for contemporary spaces.
            </p>

          </div>

        </div>


        <div class="product">

          <img
            src="https://images.unsplash.com/photo-1618220179428-22790b461013?auto=format&fit=crop&w=900&q=80"
            alt="Premium surface"
          >

          <div class="product-content">

            <div class="product-category">
              Premium Surface
            </div>

            <h3>Travertine</h3>

            <p>
              Natural texture and warmth for timeless interiors.
            </p>

          </div>

        </div>

      </div>

    </div>

  </section>


  <!-- SCHEDULE MEETING -->

  <section class="meeting" id="meeting">

    <div class="container">

      <div class="meeting-wrapper">

        <div class="hero-small">
          Private Consultation
        </div>

        <h2 class="section-title">
          Schedule a meeting.
        </h2>

        <div class="gold-line" style="margin-left:auto;margin-right:auto;"></div>

        <p class="section-subtitle">
          Choose your preferred date and time, tell us a little about
          your project, and our team will contact you to confirm your
          appointment.
        </p>


        <div class="meeting-box">

          <h3>
            Meeting Request
          </h3>


          <form id="meetingForm">

            <div class="form-grid">


              <!-- DATE -->

              <div class="form-group">

                <label for="date">
                  Preferred Date *
                </label>

                <input
                  type="date"
                  id="date"
                  required
                >

              </div>


              <!-- TIME -->

              <div class="form-group">

                <label for="time">
                  Preferred Time *
                </label>

                <select id="time" required>

                  <option value="">
                    Select time
                  </option>

                  <option value="10:00 AM">
                    10:00 AM
                  </option>

                  <option value="11:00 AM">
                    11:00 AM
                  </option>

                  <option value="12:00 PM">
                    12:00 PM
                  </option>

                  <option value="2:00 PM">
                    2:00 PM
                  </option>

                  <option value="3:00 PM">
                    3:00 PM
                  </option>

                  <option value="4:00 PM">
                    4:00 PM
                  </option>

                  <option value="5:00 PM">
                    5:00 PM
                  </option>

                  <option value="6:00 PM">
                    6:00 PM
                  </option>

                </select>

              </div>


              <!-- NAME -->

              <div class="form-group">

                <label for="name">
                  Full Name *
                </label>

                <input
                  type="text"
                  id="name"
                  placeholder="Your full name"
                  required
                >

              </div>


              <!-- PHONE -->

              <div class="form-group">

                <label for="phone">
                  Contact Number *
                </label>

                <input
                  type="tel"
                  id="phone"
                  placeholder="+91"
                  required
                >

              </div>


              <!-- EMAIL -->

              <div class="form-group">

                <label for="email">
                  Email Address
                </label>

                <input
                  type="email"
                  id="email"
                  placeholder="your@email.com"
                >

              </div>


              <!-- PROJECT -->

              <div class="form-group">

                <label for="project">
                  Project Type
                </label>

                <select id="project">

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


              <!-- MESSAGE -->

              <div class="form-group full">

                <label for="message">
                  Tell us about your requirement
                </label>

                <textarea
                  id="message"
                  placeholder="Tell us about your project or tile requirement..."
                ></textarea>

              </div>


            </div>


            <button
              type="submit"
              class="submit-button"
            >
              Request Meeting
            </button>


            <div class="notice">
              After submitting, your meeting details will be prepared
              for WhatsApp confirmation.
            </div>

          </form>

        </div>

      </div>

    </div>

  </section>


  <!-- CONTACT -->

  <section class="contact" id="contact">

    <div class="container contact-grid">

      <div>

        <div class="hero-small">
          Contact Bala Surfaces
        </div>

        <h2 class="section-title">
          Let's talk about your space.
        </h2>

        <div class="gold-line"></div>

        <p class="section-subtitle">
          Have a question about our tiles or surfaces?
          Contact our team directly.
        </p>

      </div>


      <div>

        <div class="contact-item">

          <strong>
            Phone
          </strong>

          <a href="tel:+919650285586">
            +91 96502 85586
          </a>

        </div>


        <div class="contact-item">

          <strong>
            Email
          </strong>

          <a href="mailto:balasurfaces26@gmail.com">
            balasurfaces26@gmail.com
          </a>

        </div>


        <div class="contact-item">

          <strong>
            Location
          </strong>

          <span>
            Delhi, India
          </span>

        </div>


        <div class="contact-item">

          <strong>
            WhatsApp
          </strong>

          <a
            href="https://wa.me/919650285586"
            target="_blank"
          >
            Chat with Bala Surfaces
          </a>

        </div>

      </div>

    </div>

  </section>


  <!-- FOOTER -->

  <footer>

    <div class="footer-logo">
      Bala Surfaces
    </div>

    <p>
      Premium wall tiles, floor tiles & surfaces in Delhi.
    </p>

    <p style="margin-top:15px;">
      © <span id="year"></span> Bala Surfaces. All rights reserved.
    </p>

  </footer>


  <!-- WHATSAPP BUTTON -->

  <a
    href="https://wa.me/919650285586"
    target="_blank"
    class="whatsapp"
    title="WhatsApp Bala Surfaces"
  >
    ☎
  </a>


  <script>

    /* =========================
       SET CURRENT YEAR
    ========================= */

    document.getElementById("year").textContent =
      new Date().getFullYear();


    /* =========================
       PREVENT PAST DATES
    ========================= */

    const dateInput =
      document.getElementById("date");

    const today =
      new Date();

    const year =
      today.getFullYear();

    const month =
      String(today.getMonth() + 1).padStart(2, "0");

    const day =
      String(today.getDate()).padStart(2, "0");

    dateInput.min =
      `${year}-${month}-${day}`;


    /* =========================
       MEETING FORM
    ========================= */

    document
      .getElementById("meetingForm")
      .addEventListener("submit", function(event) {

        event.preventDefault();


        const date =
          document.getElementById("date").value;

        const time =
          document.getElementById("time").value;

        const name =
          document.getElementById("name").value;

        const phone =
          document.getElementById("phone").value;

        const email =
          document.getElementById("email").value;

        const project =
          document.getElementById("project").value;

        const message =
          document.getElementById("message").value;


        /* Format date */

        const selectedDate =
          new Date(date + "T00:00:00");

        const formattedDate =
          selectedDate.toLocaleDateString(
            "en-IN",
            {
              weekday: "long",
              day: "numeric",
              month: "long",
              year: "numeric"
            }
          );


        /* Create WhatsApp message */

        const whatsappMessage =

`Hello Bala Surfaces,

I would like to schedule a meeting.

Customer Details:

Name: ${name}

Phone: ${phone}

Email: ${email || "Not provided"}

Project Type: ${project}

Preferred Date: ${formattedDate}

Preferred Time: ${time}

Requirement:
${message || "Not provided"}

Please contact me to confirm the meeting.`;


        /* WhatsApp URL */

        const whatsappURL =
          "https://wa.me/919650285586?text=" +
          encodeURIComponent(whatsappMessage);


        /*
          Open WhatsApp
        */

        window.open(
          whatsappURL,
          "_blank"
        );


        /*
          Confirmation message
        */

        alert(
          "Thank you, " +
          name +
          "! Your meeting request has been prepared. Please send the WhatsApp message to Bala Surfaces to complete your request."
        );

      });

  </script>

</body>
</html>
