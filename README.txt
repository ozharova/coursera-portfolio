<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Olzhas — responsive web developer portfolio">
  <title>Olzhas | Web Developer Portfolio</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <a class="skip-link" href="#main">Skip to main content</a>

  <header class="site-header">
    <nav class="nav container" aria-label="Main navigation">
      <a class="logo" href="#home" aria-label="Olzhas home">O.</a>
      <button class="menu-toggle" type="button" aria-expanded="false" aria-controls="menu">
        <span></span><span></span><span></span>
        <span class="sr-only">Open navigation menu</span>
      </button>
      <ul id="menu" class="nav-links">
        <li><a href="#home">Home</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#skills">Skills</a></li>
        <li><a href="#projects">Projects</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <main id="main">
    <section id="home" class="hero" aria-labelledby="hero-title">
      <div class="container hero-grid">
        <div>
          <p class="eyebrow">WEB DEVELOPER • DESIGN • FRONT-END</p>
          <h1 id="hero-title">Hi, I'm <span>Olzhas</span>.</h1>
          <p class="hero-text">
            I create clean, responsive and accessible websites with a focus on
            useful interfaces and simple user experiences.
          </p>
          <div class="hero-actions">
            <a class="button primary" href="#projects">View my work</a>
            <a class="button secondary" href="#contact">Contact me</a>
          </div>
        </div>
        <div class="hero-card" aria-label="Portfolio introduction">
          <div class="avatar">O</div>
          <p>Creative developer</p>
          <strong>Building ideas for the web.</strong>
        </div>
      </div>
    </section>

    <section id="about" class="section" aria-labelledby="about-title">
      <div class="container two-column">
        <div>
          <p class="eyebrow">ABOUT ME</p>
          <h2 id="about-title">Turning ideas into simple digital experiences.</h2>
        </div>
        <div class="section-copy">
          <p>
            I enjoy combining design and technology to build websites and
            applications that are clear, practical and easy to use.
          </p>
          <p>
            My approach is mobile-first: I start with a simple structure,
            improve the visual hierarchy, and then make sure the experience
            works well across phones, tablets and desktop screens.
          </p>
          <ul class="facts" aria-label="Highlights">
            <li><strong>Responsive</strong><span>Mobile-first layouts</span></li>
            <li><strong>Accessible</strong><span>Semantic HTML and clear contrast</span></li>
            <li><strong>Interactive</strong><span>JavaScript enhancements</span></li>
          </ul>
        </div>
      </div>
    </section>

    <section id="skills" class="section muted" aria-labelledby="skills-title">
      <div class="container">
        <p class="eyebrow">SKILLS</p>
        <h2 id="skills-title">What I work with</h2>
        <div class="skill-grid">
          <article class="skill-card"><span class="skill-icon">01</span><h3>HTML5</h3><p>Semantic structure and accessible content.</p></article>
          <article class="skill-card"><span class="skill-icon">02</span><h3>CSS3</h3><p>Responsive layouts, animation and visual design.</p></article>
          <article class="skill-card"><span class="skill-icon">03</span><h3>JavaScript</h3><p>Interactive components and DOM manipulation.</p></article>
          <article class="skill-card"><span class="skill-icon">04</span><h3>Responsive Design</h3><p>Layouts that adapt to mobile, tablet and desktop.</p></article>
        </div>
      </div>
    </section>

    <section id="projects" class="section" aria-labelledby="projects-title">
      <div class="container">
        <div class="section-heading">
          <div>
            <p class="eyebrow">SELECTED WORK</p>
            <h2 id="projects-title">Projects</h2>
          </div>
          <p>Three examples of digital products and web experiences.</p>
        </div>

        <div class="project-grid">
          <article class="project-card">
            <img src="assets/project-1.svg" alt="Abstract illustration for a finance dashboard">
            <div class="project-body">
              <p class="project-number">01 / FINANCE</p>
              <h3>Finance Dashboard</h3>
              <p>A clean interface concept for tracking accounts, budgets and personal finances.</p>
              <a href="#contact" class="text-link">Ask about the project →</a>
            </div>
          </article>

          <article class="project-card">
            <img src="assets/project-2.svg" alt="Abstract illustration for a social gaming platform">
            <div class="project-body">
              <p class="project-number">02 / SOCIAL</p>
              <h3>Play Bro</h3>
              <p>A social gaming concept focused on rooms, friends, voice communication and mini-games.</p>
              <a href="#contact" class="text-link">Ask about the project →</a>
            </div>
          </article>

          <article class="project-card">
            <img src="assets/project-3.svg" alt="Abstract illustration for an IT services website">
            <div class="project-body">
              <p class="project-number">03 / WEB</p>
              <h3>IT Services Website</h3>
              <p>A modern business website concept for presenting digital services and solutions.</p>
              <a href="#contact" class="text-link">Ask about the project →</a>
            </div>
          </article>
        </div>
      </div>
    </section>

    <section id="contact" class="section contact-section" aria-labelledby="contact-title">
      <div class="container contact-box">
        <div>
          <p class="eyebrow">GET IN TOUCH</p>
          <h2 id="contact-title">Have an idea?</h2>
          <p>I'd be happy to hear about it.</p>
        </div>
        <form id="contact-form" class="contact-form">
          <label for="name">Name</label>
          <input id="name" name="name" type="text" autocomplete="name" required>

          <label for="email">Email</label>
          <input id="email" name="email" type="email" autocomplete="email" required>

          <label for="message">Message</label>
          <textarea id="message" name="message" rows="4" required></textarea>

          <button class="button primary" type="submit">Send message</button>
          <p id="form-message" class="form-message" role="status" aria-live="polite"></p>
        </form>
      </div>
    </section>
  </main>

  <footer class="footer">
    <div class="container footer-inner">
      <p>© <span id="year"></span> Olzhas. Built as a responsive portfolio.</p>
      <a href="#home">Back to top ↑</a>
    </div>
  </footer>

  <script src="script.js"></script>
</body>
</html>
