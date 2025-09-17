# Html-website-project-
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1">

  <!-- Primary SEO -->
  <title>Ibra Tech Solutions — Web & Social Media Portfolio</title>
  <meta name="description" content="Ibra Tech Solutions — professional web design, development, and social media marketing services. Portfolio showcasing projects, services, and contact information.">
  <link rel="canonical" href="https://www.example.com/">

  <!-- Open Graph (for social sharing) -->
  <meta property="og:title" content="Ibra Tech Solutions — Web & Social Media Portfolio">
  <meta property="og:description" content="Web design, development, and social media marketing portfolio and services from Ibra Tech Solutions.">
  <meta property="og:type" content="website">
  <meta property="og:url" content="https://www.example.com/">
  <meta property="og:image" content="https://www.example.com/og-image.jpg">

  <!-- Twitter card -->
  <meta name="twitter:card" content="summary_large_image">
  <meta name="twitter:site" content="@IbraTech">

  <!-- Structured data (JSON-LD) for SEO -->
  <script type="application/ld+json">
  {
    "@context": "https://schema.org",
    "@type": "Organization",
    "name": "Ibra Tech Solutions",
    "url": "https://www.example.com/",
    "logo": "https://www.example.com/logo.png",
    "sameAs": ["https://www.facebook.com/ibra","https://www.linkedin.com/company/ibra-tech"]
  }
  </script>

  <!-- Styles (kept simple so this is a single file) -->
  <style>
    :root{--accent:#1e88e5;--max-width:1000px}
    html{font-family:system-ui,-apple-system,Segoe UI,Roboto,'Helvetica Neue',Arial;line-height:1.45}
    body{margin:0;color:#111;background:#fff}
    .container{max-width:var(--max-width);margin:0 auto;padding:1rem}
    header, nav, main, footer, aside, section, article{display:block}
    header{padding:1rem 0;border-bottom:1px solid #eee}
    .brand{font-weight:700;font-size:1.25rem}
    nav ul{list-style:none;padding:0;margin:0;display:flex;gap:0.75rem}
    nav a{color:var(--accent);text-decoration:none}
    .hero{padding:2rem 0}
    .grid{display:grid;grid-template-columns:1fr;gap:1rem}
    @media(min-width:760px){.grid{grid-template-columns:2fr 1fr}}
    .card{border:1px solid #eee;padding:1rem;border-radius:8px}
    .sr-only{position:absolute;left:-10000px;top:auto;width:1px;height:1px;overflow:hidden}
    a.skip-link{position:absolute;left:0;top:-40px;background:#000;color:#fff;padding:0.5rem;z-index:100;transition:top .2s}
    a.skip-link:focus{top:0}
    footer{padding:1rem 0;border-top:1px solid #eee;margin-top:2rem}
  </style>
</head>
<body>
  <!-- Skip link for keyboard users -->
  <a href="#main-content" class="skip-link">Skip to main content</a>

  <div class="container">
    <header role="banner">
      <div style="display:flex;align-items:center;justify-content:space-between;gap:1rem">
        <div>
          <a href="/" class="brand" aria-label="Ibra Tech Solutions home">Ibra Tech Solutions</a>
          <p class="sr-only">Providing web design & social media marketing services</p>
        </div>

        <nav role="navigation" aria-label="Primary navigation">
          <ul>
            <li><a href="#about">About</a></li>
            <li><a href="#services">Services</a></li>
            <li><a href="#work">Work</a></li>
            <li><a href="#contact">Contact</a></li>
          </ul>
        </nav>
      </div>
    </header>

    <main id="main-content" role="main">
      <article aria-labelledby="page-title">
        <header class="hero">
          <h1 id="page-title">Professional Web Design & Social Media Marketing</h1>
          <p>We build accessible websites and engaging social content that helps businesses grow online.</p>
        </header>

        <section id="about" aria-labelledby="about-heading">
          <h2 id="about-heading">About Ibra Tech Solutions</h2>
          <p>We specialise in WordPress websites, graphic design, and social media strategies for Instagram, Facebook and TikTok. Our focus is reliable delivery, clean design, and measurable results.</p>
        </section>

        <section id="services" aria-labelledby="services-heading">
          <h2 id="services-heading">Services</h2>
          <ul>
            <li><strong>Web Design & Development</strong> — Responsive, accessible sites with fast performance.</li>
            <li><strong>Social Media Marketing</strong> — Content strategy and paid campaigns for growth.</li>
            <li><strong>Branding & Graphics</strong> — Logos, visual identity, and marketing materials.</li>
          </ul>
        </section>

        <section id="work" aria-labelledby="work-heading">
          <h2 id="work-heading">Selected Projects</h2>

          <div class="grid">
            <div class="card" role="region" aria-labelledby="project-1-title">
              <h3 id="project-1-title">Portfolio Website for Local NGO</h3>
              <p>Designed an accessible WordPress site with clear donation and volunteer funnels.</p>
            </div>

            <aside class="card" role="complementary" aria-labelledby="testimonials-heading">
              <h3 id="testimonials-heading">Testimonials</h3>
              <p>"Great work — delivered on time and improved our online donations." — Client</p>
            </aside>
          </div>
        </section>

        <section id="contact" aria-labelledby="contact-heading">
          <h2 id="contact-heading">Contact</h2>
          <p>Ready to start? Fill out the form or email <a href="mailto:hello@example.com">hello@example.com</a>.</p>

          <form action="/contact" method="post" aria-label="Contact form">
            <div>
              <label for="name">Name</label>
              <input id="name" name="name" type="text" required aria-required="true">
            </div>

            <div>
              <label for="email">Email</label>
              <input id="email" name="email" type="email" required aria-required="true">
            </div>

            <div>
              <label for="message">Message</label>
              <textarea id="message" name="message" rows="5"></textarea>
            </div>

            <div>
              <button type="submit">Send message</button>
            </div>
          </form>
        </section>

      </article>
    </main>

    <footer role="contentinfo">
      <p>&copy; <time datetime="2025-09-17">2025</time> Ibra Tech Solutions. <a href="#" aria-label="Privacy policy">Privacy policy</a></p>
    </footer>
  </div>

  <!-- Small script to enhance accessibility: focus visible outline for keyboard users -->
  <script>
    (function(){
      function handleFirstTab(e){
        if(e.key === 'Tab'){
          document.documentElement.classList.add('user-is-tabbing');
          window.removeEventListener('keydown', handleFirstTab);
        }
      }
      window.addEventListener('keydown', handleFirstTab);
    })();
  </script>
</body>
</html>
