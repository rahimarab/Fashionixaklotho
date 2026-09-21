# Fashionixaklotho
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <meta name="description" content="Fashionixa Klotho - Custom apparel printing for individuals, businesses, schools, events and organizations across the USA.">

  <title>Fashionixa Klotho | Custom Apparel Printing</title>

  <style>
    :root {
      --green: #16a34a;
      --dark-green: #0f7a35;
      --black: #0b0b0b;
      --dark: #171717;
      --light: #f4f7f5;
      --white: #ffffff;
      --text: #222222;
      --gray: #666666;
      --border: #e1e7e3;
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
      font-family: Arial, Helvetica, sans-serif;
      color: var(--text);
      line-height: 1.6;
      background: white;
    }

    a {
      text-decoration: none;
      color: inherit;
    }

    .container {
      width: 92%;
      max-width: 1150px;
      margin: auto;
    }

    /* TOP BAR */
    .topbar {
      background: var(--black);
      color: white;
      text-align: center;
      padding: 9px 15px;
      font-size: 14px;
    }

    /* NAVIGATION */
    .navbar {
      background: white;
      border-bottom: 1px solid var(--border);
      position: sticky;
      top: 0;
      z-index: 1000;
    }

    .nav-inner {
      min-height: 72px;
      display: flex;
      align-items: center;
      justify-content: space-between;
    }

    .logo {
      display: flex;
      align-items: center;
      gap: 10px;
      font-size: 20px;
      font-weight: 800;
    }

    .logo-mark {
      width: 42px;
      height: 42px;
      background: var(--green);
      color: white;
      display: flex;
      align-items: center;
      justify-content: center;
      border-radius: 9px;
      font-weight: 900;
    }

    .nav-links {
      display: flex;
      align-items: center;
      gap: 27px;
    }

    .nav-links a {
      font-size: 15px;
      font-weight: 700;
    }

    .nav-links a:hover {
      color: var(--green);
    }

    .menu-btn {
      display: none;
      border: none;
      background: transparent;
      font-size: 28px;
      cursor: pointer;
    }

    /* HERO */
    .hero {
      background: linear-gradient(
        135deg,
        #f1faf4,
        #ffffff 60%,
        #e8f7ed
      );
      padding: 90px 0;
    }

    .hero-grid {
      display: grid;
      grid-template-columns: 1.2fr .8fr;
      gap: 55px;
      align-items: center;
    }

    .eyebrow {
      display: inline-block;
      background: #dcfce7;
      color: var(--dark-green);
      padding: 7px 13px;
      border-radius: 30px;
      font-size: 13px;
      font-weight: 800;
      margin-bottom: 18px;
    }

    h1 {
      font-size: clamp(40px, 5vw, 65px);
      line-height: 1.05;
      color: var(--black);
      margin-bottom: 22px;
    }

    h1 span {
      color: var(--green);
    }

    .hero p {
      font-size: 19px;
      color: var(--gray);
      max-width: 680px;
      margin-bottom: 30px;
    }

    .buttons {
      display: flex;
      flex-wrap: wrap;
      gap: 12px;
    }

    .btn {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      padding: 13px 21px;
      border-radius: 8px;
      font-weight: 800;
      border: 2px solid transparent;
      cursor: pointer;
    }

    .btn-primary {
      background: var(--green);
      color: white;
    }

    .btn-primary:hover {
      background: var(--dark-green);
    }

    .btn-dark {
      background: var(--black);
      color: white;
    }

    .btn-outline {
      border-color: #bbb;
      background: white;
    }

    .btn-outline:hover {
      border-color: var(--green);
      color: var(--green);
    }

    .hero-card {
      background: white;
      padding: 30px;
      border-radius: 18px;
      border: 1px solid var(--border);
      box-shadow: 0 15px 40px rgba(0,0,0,.08);
    }

    .hero-card h3 {
      font-size: 24px;
      margin-bottom: 16px;
    }

    .check {
      display: flex;
      gap: 10px;
      margin: 12px 0;
    }

    .check b {
      color: var(--green);
    }

    /* SECTIONS */
    section {
      padding: 78px 0;
    }

    .light {
      background: var(--light);
    }

    .section-head {
      text-align: center;
      max-width: 720px;
      margin: 0 auto 42px;
    }

    .section-head h2 {
      font-size: 36px;
      line-height: 1.2;
      margin-bottom: 12px;
      color: var(--black);
    }

    .section-head p {
      color: var(--gray);
    }

    /* SERVICES */
    .grid {
      display: grid;
      gap: 20px;
    }

    .services {
      grid-template-columns: repeat(4, 1fr);
    }

    .card {
      background: white;
      border: 1px solid var(--border);
      border-radius: 14px;
      padding: 24px;
    }

    .card:hover {
      transform: translateY(-3px);
      box-shadow: 0 12px 30px rgba(0,0,0,.07);
      transition: .2s;
    }

    .icon {
      width: 45px;
      height: 45px;
      border-radius: 10px;
      background: #dcfce7;
      color: var(--dark-green);
      display: flex;
      align-items: center;
      justify-content: center;
      font-weight: 900;
      margin-bottom: 15px;
    }

    .card h3 {
      margin-bottom: 8px;
      font-size: 19px;
    }

    .card p {
      color: var(--gray);
      font-size: 15px;
    }

    /* PRINTING METHODS */
    .methods {
      grid-template-columns: repeat(5, 1fr);
    }

    .method {
      background: white;
      border: 1px solid var(--border);
      border-radius: 12px;
      padding: 24px 14px;
      text-align: center;
      font-weight: 800;
    }

    .method small {
      display: block;
      margin-top: 5px;
      color: #777;
      font-weight: normal;
    }

    /* CUSTOMERS */
    .audience {
      grid-template-columns: repeat(4, 1fr);
    }

    .audience .card {
      border-top: 4px solid var(--green);
    }

    /* STEPS */
    .steps {
      grid-template-columns: repeat(4, 1fr);
    }

    .step {
      text-align: center;
    }

    .number {
      width: 48px;
      height: 48px;
      border-radius: 50%;
      background: var(--black);
      color: white;
      display: flex;
      align-items: center;
      justify-content: center;
      margin: 0 auto 15px;
      font-weight: 900;
    }

    /* ABOUT */
    .about {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 45px;
      align-items: center;
    }

    .about-text h2 {
      font-size: 38px;
      line-height: 1.15;
      margin-bottom: 17px;
    }

    .about-text p {
      color: var(--gray);
      margin-bottom: 16px;
    }

    .highlight {
      margin: 11px 0;
      display: flex;
      gap: 10px;
    }

    .highlight span {
      color: var(--green);
      font-weight: 900;
    }

    .about-box {
      background: var(--black);
      color: white;
      border-radius: 18px;
      padding: 40px;
    }

    .about-box h3 {
      font-size: 28px;
      margin-bottom: 14px;
    }

    /* QUOTE */
    .quote-wrap {
      display: grid;
      grid-template-columns: .75fr 1.25fr;
      gap: 35px;
      align-items: start;
    }

    .quote-info {
      background: var(--black);
      color: white;
      border-radius: 18px;
      padding: 35px;
    }

    .quote-info h2 {
      font-size: 34px;
      line-height: 1.15;
      margin-bottom: 14px;
    }

    .quote-info p {
      color: #ddd;
      margin-bottom: 20px;
    }

    .contact-line {
      border-top: 1px solid #333;
      padding: 13px 0;
    }

    .form {
      background: white;
      border: 1px solid var(--border);
      border-radius: 18px;
      padding: 30px;
    }

    .form-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 17px;
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
      font-size: 14px;
      font-weight: 700;
    }

    input,
    select,
    textarea {
      width: 100%;
      padding: 12px 13px;
      border: 1px solid #ccd5cf;
      border-radius: 8px;
      font: inherit;
      background: white;
    }

    textarea {
      min-height: 120px;
      resize: vertical;
    }

    input:focus,
    select:focus,
    textarea:focus {
      outline: 2px solid #bbf7d0;
      border-color: var(--green);
    }

    .form-note {
      font-size: 13px;
      color: #777;
      margin-top: 12px;
    }

    /* CONTACT */
    .contact {
      text-align: center;
      background: #eaf7ee;
    }

    .contact-buttons {
      justify-content: center;
    }

    /* FOOTER */
    footer {
      background: var(--black);
      color: #ddd;
      padding: 30px 0;
    }

    .footer-inner {
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 20px;
    }

    .footer-links {
      display: flex;
      gap: 18px;
      font-size: 14px;
    }

    .footer-links a:hover {
      color: white;
    }

    /* MOBILE */
    @media(max-width: 900px) {

      .hero-grid,
      .about,
      .quote-wrap {
        grid-template-columns: 1fr;
      }

      .services {
        grid-template-columns: repeat(2, 1fr);
      }

      .methods {
        grid-template-columns: repeat(3, 1fr);
      }

      .audience {
        grid-template-columns: repeat(2, 1fr);
      }

      .steps {
        grid-template-columns: repeat(2, 1fr);
      }
    }

    @media(max-width: 700px) {

      .menu-btn {
        display: block;
      }

      .nav-links {
        display: none;
        position: absolute;
        top: 72px;
        left: 0;
        right: 0;
        background: white;
        border-bottom: 1px solid var(--border);
        padding: 15px 4%;
        flex-direction: column;
        align-items: flex-start;
      }

      .nav-links.open {
        display: flex;
      }

      .hero {
        padding: 60px 0;
      }

      section {
        padding: 58px 0;
      }

      .services,
      .methods,
      .audience,
      .steps {
        grid-template-columns: 1fr;
      }

      .form-grid {
        grid-template-columns: 1fr;
      }

      .field.full {
        grid-column: auto;
      }

      .footer-inner {
        flex-direction: column;
        text-align: center;
      }

      .footer-links {
        flex-wrap: wrap;
        justify-content: center;
      }
    }
  </style>
</head>

<body>

  <!-- TOP BAR -->
  <div class="topbar">
    Custom Apparel Printing • Small Orders & Bulk Orders • Serving Customers Across the USA
  </div>

  <!-- NAVIGATION -->
  <header class="navbar">
    <div class="container nav-inner">

      <a href="#home" class="logo">
        <span class="logo-mark">FK</span>
        <span>Fashionixa Klotho</span>
      </a>

      <button class="menu-btn" onclick="toggleMenu()">☰</button>

      <nav class="nav-links" id="navLinks">
        <a href="#services" onclick="closeMenu()">Services</a>
        <a href="#methods" onclick="closeMenu()">Printing</a>
        <a href="#about" onclick="closeMenu()">About</a>
        <a href="#quote" onclick="closeMenu()">Get a Quote</a>
        <a href="#contact" onclick="closeMenu()">Contact</a>
      </nav>

    </div>
  </header>


  <!-- HERO -->
  <section class="hero" id="home">

    <div class="container hero-grid">

      <div>

        <div class="eyebrow">
          CUSTOM APPAREL PRINTING
        </div>

        <h1>
          Custom Apparel Printing for
          <span>Individuals & Businesses</span>
        </h1>

        <p>
          Turn your ideas, logos, and designs into quality custom apparel.
          We offer flexible options for individuals, businesses, schools,
          events, organizations, and bulk orders.
        </p>

        <div class="buttons">

          <a href="#quote" class="btn btn-primary">
            Get a Free Quote
          </a>

          <a href="tel:+12149237638" class="btn btn-dark">
            Call 214-923-7638
          </a>

        </div>

      </div>


      <div class="hero-card">

        <h3>What We Print</h3>

        <div class="check">
          <b>✓</b>
          <span>T-Shirts & Hoodies</span>
        </div>

        <div class="check">
          <b>✓</b>
          <span>Polos & Work Apparel</span>
        </div>

        <div class="check">
          <b>✓</b>
          <span>School & Graduation Shirts</span>
        </div>

        <div class="check">
          <b>✓</b>
          <span>Event & Party Shirts</span>
        </div>

        <div class="check">
          <b>✓</b>
          <span>Business & Company Apparel</span>
        </div>

        <div class="check">
          <b>✓</b>
          <span>Small & Bulk Orders</span>
        </div>

      </div>

    </div>

  </section>


  <!-- SERVICES -->
  <section id="services">

    <div class="container">

      <div class="section-head">

        <h2>Our Custom Apparel Services</h2>

        <p>
          Choose the apparel and printing option that fits your project.
        </p>

      </div>


      <div class="grid services">

        <div class="card">
          <div class="icon">01</div>
          <h3>T-Shirts</h3>
          <p>
            Custom shirts for personal use, teams, businesses,
            events, and promotions.
          </p>
        </div>


        <div class="card">
          <div class="icon">02</div>
          <h3>Hoodies & Sweatshirts</h3>
          <p>
            Custom printed hoodies and sweatshirts for brands,
            groups, and everyday wear.
          </p>
        </div>


        <div class="card">
          <div class="icon">03</div>
          <h3>Polos</h3>
          <p>
            Professional custom polos for businesses,
            teams, schools, and organizations.
          </p>
        </div>


        <div class="card">
          <div class="icon">04</div>
          <h3>Work Uniforms</h3>
          <p>
            Custom business apparel that helps your team
            look consistent and professional.
          </p>
        </div>


        <div class="card">
          <div class="icon">05</div>
          <h3>School & Graduation</h3>
          <p>
            Class shirts, graduation apparel, school events,
            clubs, and student groups.
          </p>
        </div>


        <div class="card">
          <div class="icon">06</div>
          <h3>Events & Parties</h3>
          <p>
            Matching shirts for birthdays, reunions,
            celebrations, and special events.
          </p>
        </div>


        <div class="card">
          <div class="icon">07</div>
          <h3>Business Apparel</h3>
          <p>
            Logo shirts, branded apparel, promotional clothing,
            and company orders.
          </p>
        </div>


        <div class="card">
          <div class="icon">08</div>
          <h3>Bulk Orders</h3>
          <p>
            Flexible solutions for larger orders and
            organizations with recurring apparel needs.
          </p>
        </div>

      </div>

    </div>

  </section>


  <!-- PRINTING METHODS -->
  <section id="methods" class="light">

    <div class="container">

      <div class="section-head">

        <h2>Printing Methods</h2>

        <p>
          We match your order with the printing method
          that fits your design, quantity, and apparel.
        </p>

      </div>


      <div class="grid methods">

        <div class="method">
          DTF
          <small>Flexible custom prints</small>
        </div>

        <div class="method">
          Screen Printing
          <small>Great for bulk orders</small>
        </div>

        <div class="method">
          DTG
          <small>Detailed full-color designs</small>
        </div>

        <div class="method">
          Vinyl
          <small>Names, numbers & graphics</small>
        </div>

        <div class="method">
          Custom Options
          <small>Ask us for a quote</small>
        </div>

      </div>

    </div>

  </section>


  <!-- CUSTOMERS -->
  <section>

    <div class="container">

      <div class="section-head">

        <h2>Who We Serve</h2>

        <p>
          From one custom shirt to large company orders.
        </p>

      </div>


      <div class="grid audience">

        <div class="card">
          <h3>Individuals</h3>
          <p>
            Personal shirts, gifts, family designs,
            and custom apparel.
          </p>
        </div>


        <div class="card">
          <h3>Small Businesses</h3>
          <p>
            Branded shirts, uniforms, promotional apparel,
            and staff clothing.
          </p>
        </div>


        <div class="card">
          <h3>Schools & Events</h3>
          <p>
            Graduation, school clubs, teams, parties,
            reunions, and events.
          </p>
        </div>


        <div class="card">
          <h3>Companies & Organizations</h3>
          <p>
            Bulk apparel programs and larger recurring orders.
          </p>
        </div>

      </div>

    </div>

  </section>


  <!-- HOW IT WORKS -->
  <section class="light">

    <div class="container">

      <div class="section-head">

        <h2>How It Works</h2>

        <p>
          A simple process from your idea to finished apparel.
        </p>

      </div>


      <div class="grid steps">

        <div class="step">

          <div class="number">1</div>

          <h3>Send Your Details</h3>

          <p>
            Tell us what you need and upload your artwork.
          </p>

        </div>


        <div class="step">

          <div class="number">2</div>

          <h3>Get Your Quote</h3>

          <p>
            We review your order and provide pricing.
          </p>

        </div>


        <div class="step">

          <div class="number">3</div>

          <h3>Approve</h3>

          <p>
            Confirm your order details and production plan.
          </p>

        </div>


        <div class="step">

          <div class="number">4</div>

          <h3>Print & Deliver</h3>

          <p>
            Most orders are completed within 5–7 business days.
          </p>

        </div>

      </div>

    </div>

  </section>


  <!-- ABOUT -->
  <section id="about">

    <div class="container about">

      <div class="about-text">

        <h2>About Fashionixa Klotho</h2>

        <p>
          Fashionixa Klotho is a custom apparel printing company
          serving individuals, businesses, schools, events,
          and organizations across the USA.
        </p>

        <p>
          We make it easy to turn your ideas and designs into
          custom apparel, with flexible options for both small
          and bulk orders.
        </p>


        <div class="highlight">
          <span>✓</span>
          Small and bulk orders
        </div>

        <div class="highlight">
          <span>✓</span>
          Multiple printing methods
        </div>

        <div class="highlight">
          <span>✓</span>
          USA-wide shipping available
        </div>

        <div class="highlight">
          <span>✓</span>
          Free quotes
        </div>

      </div>


      <div class="about-box">

        <h3>Need apparel for your business?</h3>

        <p>
          Send us your logo, quantity, apparel type,
          and deadline. We'll review your project
          and provide a quote.
        </p>

        <br>

        <a href="#quote" class="btn btn-primary">
          Request a Quote
        </a>

      </div>

    </div>

  </section>


  <!-- QUOTE FORM -->
  <section id="quote" class="light">

    <div class="container quote-wrap">


      <div class="quote-info">

        <h2>Get Your Free Quote</h2>

        <p>
          Tell us about your order. You can upload your artwork
          and we'll contact you with the next steps.
        </p>


        <div class="contact-line">
          <strong>Phone</strong><br>
          <a href="tel:+12149237638">
            214-923-7638
          </a>
        </div>


        <div class="contact-line">
          <strong>Email</strong><br>
          <a href="mailto:Info.fashionixaklotho@gmail.com">
            Info.fashionixaklotho@gmail.com
          </a>
        </div>


        <div class="contact-line">
          <strong>WhatsApp</strong><br>
          <a
            href="https://wa.me/12149237638"
            target="_blank"
          >
            Chat on WhatsApp
          </a>
        </div>


        <div class="contact-line">
          <strong>Service Area</strong><br>
          Dallas & Customers Across the USA
        </div>

      </div>


      <form
        class="form"
        id="quoteForm"
        onsubmit="sendQuote(event)"
      >

        <div class="form-grid">


          <div class="field">

            <label>Full Name *</label>

            <input
              id="name"
              type="text"
              required
            >

          </div>


          <div class="field">

            <label>Business / Organization</label>

            <input
              id="business"
              type="text"
            >

          </div>


          <div class="field">

            <label>Phone *</label>

            <input
              id="phone"
              type="tel"
              required
            >

          </div>


          <div class="field">

            <label>Email *</label>

            <input
              id="email"
              type="email"
              required
            >

          </div>


          <div class="field">

            <label>Product *</label>

            <select id="product" required>

              <option value="">
                Select
              </option>

              <option>T-Shirt</option>
              <option>Hoodie / Sweatshirt</option>
              <option>Polo</option>
              <option>Work Uniform</option>
              <option>School / Graduation</option>
              <option>Event / Party</option>
              <option>Business Apparel</option>
              <option>Other</option>

            </select>

          </div>


          <div class="field">

            <label>Quantity *</label>

            <input
              id="quantity"
              type="number"
              min="1"
              required
            >

          </div>


          <div class="field">

            <label>Printing Method</label>

            <select id="method">

              <option value="">
                Not sure
              </option>

              <option>DTF</option>
              <option>Screen Printing</option>
              <option>DTG</option>
              <option>Vinyl</option>
              <option>
                Not sure - recommend one
              </option>

            </select>

          </div>


          <div class="field">

            <label>Apparel Color</label>

            <input
              id="color"
              type="text"
              placeholder="Black, white, green..."
            >

          </div>


          <div class="field full">

            <label>Size Breakdown</label>

            <input
              id="sizes"
              type="text"
              placeholder="Example: S-2, M-5, L-8, XL-3"
            >

          </div>


          <div class="field">

            <label>Desired Deadline</label>

            <input
              id="deadline"
              type="date"
            >

          </div>


          <div class="field">

            <label>Upload Artwork</label>

            <input
              id="artwork"
              type="file"
              accept=".png,.jpg,.jpeg,.pdf,.ai,.eps,.svg"
            >

          </div>


          <div class="field full">

            <label>Additional Details</label>

            <textarea
              id="details"
              placeholder="Tell us about your design, placement, special requirements, etc."
            ></textarea>

          </div>

        </div>


        <button
          class="btn btn-primary"
          style="width:100%;margin-top:20px"
          type="submit"
        >
          Send Quote Request
        </button>


        <p class="form-note">
          Your email app and WhatsApp will open with your
          quote information. For now, please attach artwork
          manually to the email.
        </p>

      </form>

    </div>

  </section>


  <!-- CONTACT -->
  <section id="contact" class="contact">

    <div class="container">

      <div class="section-head">

        <h2>Let's Print Your Next Project</h2>

        <p>
          Call, email, or message us on WhatsApp for a free quote.
        </p>

      </div>


      <div class="buttons contact-buttons">

        <a href="#quote" class="btn btn-primary">
          Get a Free Quote
        </a>

        <a
          href="tel:+12149237638"
          class="btn btn-dark"
        >
          214-923-7638
        </a>

        <a
          href="https://wa.me/12149237638"
          target="_blank"
          class="btn btn-outline"
        >
          WhatsApp
        </a>

        <a
          href="https://www.facebook.com/share/1LW83hyQiu/"
          target="_blank"
          class="btn btn-outline"
        >
          Facebook
        </a>

      </div>

    </div>

  </section>


  <!-- FOOTER -->
  <footer>

    <div class="container footer-inner">

      <div>
        © <span id="year"></span>
        Fashionixa Klotho.
        All rights reserved.
      </div>


      <div class="footer-links">

        <a href="#services">Services</a>

        <a href="#quote">Get a Quote</a>

        <a href="mailto:Info.fashionixaklotho@gmail.com">
          Email
        </a>

        <a href="tel:+12149237638">
          Call
        </a>

      </div>

    </div>

  </footer>


  <!-- JAVASCRIPT -->
  <script>

    function toggleMenu() {

      document
        .getElementById("navLinks")
        .classList.toggle("open");

    }


    function closeMenu() {

      document
        .getElementById("navLinks")
        .classList.remove("open");

    }


    function sendQuote(event) {

      event.preventDefault();


      const name =
        document.getElementById("name").value;

      const business =
        document.getElementById("business").value;

      const phone =
        document.getElementById("phone").value;

      const email =
        document.getElementById("email").value;

      const product =
        document.getElementById("product").value;

      const quantity =
        document.getElementById("quantity").value;

      const method =
        document.getElementById("method").value;

      const color =
        document.getElementById("color").value;

      const sizes =
        document.getElementById("sizes").value;

      const deadline =
        document.getElementById("deadline").value;

      const details =
        document.getElementById("details").value;


      const subject =
        "New Custom Apparel Quote - " + name;


      const message =

`Hello Fashionixa Klotho,

I would like a quote for custom apparel.

Full Name: ${name}

Business / Organization:
${business}

Phone:
${phone}

Email:
${email}

Product:
${product}

Quantity:
${quantity}

Printing Method:
${method}

Apparel Color:
${color}

Size Breakdown:
${sizes}

Desired Deadline:
${deadline}

Additional Details:
${details}

Thank you.`;


      /* OPEN EMAIL */

      const emailLink =
        "mailto:Info.fashionixaklotho@gmail.com" +
        "?subject=" +
        encodeURIComponent(subject) +
        "&body=" +
        encodeURIComponent(message);


      window.location.href = emailLink;


      /* OPEN WHATSAPP */

      setTimeout(function() {

        const whatsappMessage =

`Custom Apparel Quote Request

Name: ${name}
Business: ${business}
Phone: ${phone}
Email: ${email}
Product: ${product}
Quantity: ${quantity}
Printing: ${method}
Color: ${color}
Sizes: ${sizes}
Deadline: ${deadline}

Details:
${details}`;


        window.open(
          "https://wa.me/12149237638?text=" +
          encodeURIComponent(whatsappMessage),
          "_blank"
        );

      }, 1000);

    }


    /* CURRENT YEAR */

    document.getElementById("year").textContent =
      new Date().getFullYear();

  </script>

</body>
</html>
