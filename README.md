<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Moe Kya Waung | Full-Stack Developer</title>
  <meta
    name="description"
    content="Moe Kya Waung - Full-Stack Developer specializing in Android, Web Development, and DevOps. Explore projects, skills, certifications, and contact information."
  />
  <meta name="author" content="Moe Kya Waung" />

  <meta property="og:title" content="Moe Kya Waung | Full-Stack Developer" />
  <meta
    property="og:description"
    content="Professional developer portfolio of Moe Kya Waung - Android, Web, DevOps, and Full-Stack Development."
  />
  <meta property="og:type" content="website" />
  <meta
    property="og:image"
    content="https://via.placeholder.com/1200x630/111827/ffffff?text=Moe+Kya+Waung"
  />

  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link
    href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap"
    rel="stylesheet"
  />

  <style>
    :root {
      --bg: #0b1120;
      --bg-soft: #111827;
      --card: #151d2f;
      --card-2: #1b253a;
      --text: #f8fafc;
      --muted: #94a3b8;
      --line: rgba(255, 255, 255, 0.08);
      --primary: #38bdf8;
      --primary-dark: #0ea5e9;
      --accent: #22c55e;
      --warning: #f59e0b;
      --shadow: 0 12px 40px rgba(0, 0, 0, 0.35);
      --radius: 18px;
      --max: 1120px;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      font-family: "Inter", sans-serif;
      background:
        radial-gradient(circle at top right, rgba(56, 189, 248, 0.08), transparent 25%),
        linear-gradient(180deg, #0b1120 0%, #0f172a 100%);
      color: var(--text);
      line-height: 1.6;
    }

    a {
      text-decoration: none;
      color: inherit;
    }

    .container {
      width: min(var(--max), calc(100% - 2rem));
      margin: 0 auto;
    }

    header {
      position: sticky;
      top: 0;
      z-index: 100;
      background: rgba(11, 17, 32, 0.8);
      backdrop-filter: blur(14px);
      border-bottom: 1px solid var(--line);
    }

    .nav {
      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: 1rem;
      padding: 1rem 0;
    }

    .logo {
      font-size: 1.15rem;
      font-weight: 800;
      letter-spacing: 0.2px;
    }

    .logo span {
      color: var(--primary);
    }

    .nav-links {
      display: flex;
      flex-wrap: wrap;
      gap: 1rem;
    }

    .nav-links a {
      color: var(--muted);
      font-weight: 500;
      transition: 0.2s ease;
    }

    .nav-links a:hover {
      color: var(--text);
    }

    .hero {
      padding: 5rem 0 4rem;
    }

    .hero-grid {
      display: grid;
      grid-template-columns: 1.2fr 0.8fr;
      gap: 2rem;
      align-items: center;
    }

    .badge {
      display: inline-block;
      background: rgba(56, 189, 248, 0.12);
      color: #bae6fd;
      border: 1px solid rgba(56, 189, 248, 0.2);
      padding: 0.45rem 0.8rem;
      border-radius: 999px;
      font-size: 0.85rem;
      font-weight: 700;
      margin-bottom: 1rem;
    }

    h1 {
      font-size: clamp(2.4rem, 5vw, 4.2rem);
      line-height: 1.1;
      margin-bottom: 1rem;
    }

    .hero p {
      color: var(--muted);
      font-size: 1.05rem;
      max-width: 62ch;
    }

    .hero-actions {
      display: flex;
      gap: 1rem;
      flex-wrap: wrap;
      margin-top: 1.75rem;
    }

    .btn {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      padding: 0.9rem 1.25rem;
      border-radius: 12px;
      font-weight: 600;
      transition: 0.2s ease;
      border: 1px solid transparent;
    }

    .btn-primary {
      background: linear-gradient(135deg, var(--primary), var(--primary-dark));
      color: white;
      box-shadow: var(--shadow);
    }

    .btn-primary:hover {
      transform: translateY(-2px);
      opacity: 0.96;
    }

    .btn-secondary {
      background: rgba(255, 255, 255, 0.03);
      border: 1px solid var(--line);
      color: var(--text);
    }

    .btn-secondary:hover {
      transform: translateY(-2px);
      border-color: rgba(255, 255, 255, 0.18);
    }

    .hero-card {
      background: linear-gradient(180deg, var(--card), var(--card-2));
      border: 1px solid var(--line);
      border-radius: 24px;
      padding: 1.5rem;
      box-shadow: var(--shadow);
    }

    .avatar {
      width: 88px;
      height: 88px;
      border-radius: 22px;
      display: grid;
      place-items: center;
      background: linear-gradient(135deg, var(--primary), var(--accent));
      color: white;
      font-size: 2rem;
      font-weight: 800;
      margin-bottom: 1rem;
    }

    .hero-card h2 {
      font-size: 1.3rem;
      margin-bottom: 0.5rem;
    }

    .meta {
      list-style: none;
      display: grid;
      gap: 0.75rem;
      color: var(--muted);
      margin-top: 1rem;
      font-size: 0.96rem;
    }

    section {
      padding: 4rem 0;
    }

    .section-heading {
      margin-bottom: 1.75rem;
    }

    .section-heading h2 {
      font-size: 2rem;
      margin-bottom: 0.6rem;
    }

    .section-heading p {
      color: var(--muted);
      max-width: 70ch;
    }

    .cards {
      display: grid;
      gap: 1.25rem;
    }

    .skills-grid {
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
    }

    .card {
      background: linear-gradient(180deg, var(--card), var(--card-2));
      border: 1px solid var(--line);
      border-radius: var(--radius);
      padding: 1.25rem;
      box-shadow: var(--shadow);
    }

    .card h3 {
      margin-bottom: 0.6rem;
      font-size: 1.05rem;
    }

    .card p {
      color: var(--muted);
      font-size: 0.95rem;
    }

    .projects-grid {
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    }

    .project-card {
      background: linear-gradient(180deg, var(--card), var(--card-2));
      border: 1px solid var(--line);
      border-radius: 20px;
      overflow: hidden;
      box-shadow: var(--shadow);
      transition: 0.2s ease;
    }

    .project-card:hover {
      transform: translateY(-4px);
    }

    .project-top {
      height: 8px;
      background: linear-gradient(90deg, var(--primary), var(--accent));
    }

    .project-body {
      padding: 1.25rem;
    }

    .project-body h3 {
      margin-bottom: 0.6rem;
    }

    .project-body p {
      color: var(--muted);
      font-size: 0.95rem;
    }

    .tags {
      display: flex;
      flex-wrap: wrap;
      gap: 0.5rem;
      margin: 1rem 0;
    }

    .tag {
      padding: 0.35rem 0.7rem;
      border-radius: 999px;
      font-size: 0.8rem;
      font-weight: 600;
      border: 1px solid rgba(56, 189, 248, 0.18);
      background: rgba(56, 189, 248, 0.1);
      color: #bae6fd;
    }

    .links {
      display: flex;
      gap: 1rem;
      flex-wrap: wrap;
      margin-top: 0.75rem;
    }

    .links a {
      color: var(--primary);
      font-weight: 600;
      font-size: 0.94rem;
    }

    .timeline {
      display: grid;
      gap: 1rem;
    }

    .timeline-item {
      background: linear-gradient(180deg, var(--card), var(--card-2));
      border: 1px solid var(--line);
      border-radius: var(--radius);
      padding: 1.1rem 1.2rem;
      box-shadow: var(--shadow);
    }

    .timeline-item h3 {
      margin-bottom: 0.4rem;
      font-size: 1rem;
    }

    .timeline-item p {
      color: var(--muted);
      font-size: 0.95rem;
    }

    .contact-box {
      background: linear-gradient(180deg, var(--card), var(--card-2));
      border: 1px solid var(--line);
      border-radius: 24px;
      padding: 2rem;
      box-shadow: var(--shadow);
    }

    .contact-list {
      list-style: none;
      display: grid;
      gap: 0.85rem;
      margin-top: 1rem;
    }

    .contact-list a {
      color: var(--primary);
    }

    footer {
      text-align: center;
      color: var(--muted);
      border-top: 1px solid var(--line);
      padding: 1.5rem 0 3rem;
      margin-top: 2rem;
    }

    @media (max-width: 860px) {
      .hero-grid {
        grid-template-columns: 1fr;
      }

      .nav {
        flex-direction: column;
        align-items: flex-start;
      }
    }
  </style>
</head>
<body>
  <header>
    <div class="container nav">
      <a href="#" class="logo">Moe Kya Waung<span>.</span></a>
      <nav class="nav-links">
        <a href="#about">About</a>
        <a href="#skills">Skills</a>
        <a href="#projects">Projects</a>
        <a href="#certifications">Certifications</a>
        <a href="#contact">Contact</a>
        <a href="https://github.com/moekyawaung-designer" target="_blank">GitHub</a>
      </nav>
    </div>
  </header>

  <main>
    <section class="hero">
      <div class="container hero-grid">
        <div>
          <span class="badge">Full-Stack Developer</span>
          <h1>Building practical software for web, mobile, and deployment workflows.</h1>
          <p>
            I’m Moe Kya Waung, a developer focused on Android development, web applications,
            backend systems, and DevOps workflows. I enjoy building clean, useful, and maintainable solutions
            while continuously improving my technical skills.
          </p>

          <div class="hero-actions">
            <a class="btn btn-primary" href="#projects">View Projects</a>
            <a class="btn btn-secondary" href="https://github.com/moekyawaung-designer" target="_blank">GitHub Profile</a>
          </div>
        </div>

        <aside class="hero-card">
          <div class="avatar">MKW</div>
          <h2>Moe Kya Waung</h2>
          <p style="color: var(--muted);">
            Full-Stack Developer with a strong interest in Android, web engineering, backend logic, and modern deployment practices.
          </p>

          <ul class="meta">
            <li>📚 85+ certifications through continuous learning</li>
            <li>💻 Focused on Android, Web, Backend, DevOps</li>
            <li>🚀 Open to freelance, remote, and collaborative projects</li>
            <li>🌐 github.com/moekyawaung-designer</li>
          </ul>
        </aside>
      </div>
    </section>

    <section id="about">
      <div class="container">
        <div class="section-heading">
          <h2>About</h2>
          <p>
            I build software with an emphasis on clean structure, usability, and practical implementation.
            My goal is to create projects that are both professional and useful, while continuously learning
            modern tools, frameworks, and engineering best practices.
          </p>
        </div>
      </div>
    </section>

    <section id="skills">
      <div class="container">
        <div class="section-heading">
          <h2>Skills</h2>
          <p>
            A versatile technical foundation across software development, app creation, deployment, and problem solving.
          </p>
        </div>

        <div class="cards skills-grid">
          <article class="card">
            <h3>Frontend Development</h3>
            <p>HTML, CSS, JavaScript, responsive layouts, accessible UI, and clean interface structure.</p>
          </article>

          <article class="card">
            <h3>Backend Development</h3>
            <p>Server-side logic, APIs, authentication, application workflows, and structured code organization.</p>
          </article>

          <article class="card">
            <h3>Android Development</h3>
            <p>Mobile app design and development with attention to usability, structure, and practical functionality.</p>
          </article>

          <article class="card">
            <h3>DevOps & Deployment</h3>
            <p>Git, GitHub, deployment workflows, hosting, version control, and CI/CD fundamentals.</p>
          </article>

          <article class="card">
            <h3>Databases</h3>
            <p>Data modeling, storage structures, CRUD operations, and application-level data management.</p>
          </article>

          <article class="card">
            <h3>Problem Solving</h3>
            <p>Debugging, code refinement, learning by building, and improving quality through iteration.</p>
          </article>
        </div>
      </div>
    </section>

    <section id="projects">
      <div class="container">
        <div class="section-heading">
          <h2>Projects</h2>
          <p>
            Replace these examples with your real repositories and demos. Keep your best and most relevant work at the top.
          </p>
        </div>

        <div class="cards projects-grid">
          <article class="project-card">
            <div class="project-top"></div>
            <div class="project-body">
              <h3>Developer Portfolio</h3>
              <p>
                A professional GitHub Pages portfolio designed to showcase projects, technical skills, and contact details.
              </p>
              <div class="tags">
                <span class="tag">HTML</span>
                <span class="tag">CSS</span>
                <span class="tag">GitHub Pages</span>
              </div>
              <div class="links">
                <a href="https://moekyawaung-designer.github.io" target="_blank">Live Demo</a>
                <a href="https://github.com/moekyawaung-designer/moekyawaung-designer.github.io" target="_blank">Source</a>
              </div>
            </div>
          </article>

          <article class="project-card">
            <div class="project-top"></div>
            <div class="project-body">
              <h3>Android Application</h3>
              <p>
                A mobile project focused on user-friendly experience, maintainable app structure, and practical feature implementation.
              </p>
              <div class="tags">
                <span class="tag">Android</span>
                <span class="tag">Java/Kotlin</span>
                <span class="tag">Mobile UI</span>
              </div>
              <div class="links">
                <a href="#">Repository</a>
              </div>
            </div>
          </article>

          <article class="project-card">
            <div class="project-top"></div>
            <div class="project-body">
              <h3>Full-Stack Web Application</h3>
              <p>
                A complete application combining frontend interface, backend logic, and data handling into a usable solution.
              </p>
              <div class="tags">
                <span class="tag">Frontend</span>
                <span class="tag">Backend</span>
                <span class="tag">Database</span>
              </div>
              <div class="links">
                <a href="#">Repository</a>
                <a href="#">Demo</a>
              </div>
            </div>
          </article>
        </div>
      </div>
    </section>

    <section id="certifications">
      <div class="container">
        <div class="section-heading">
          <h2>Certifications</h2>
          <p>
            Highlighting continuous learning, technical development, and commitment to growth.
          </p>
        </div>

        <div class="timeline">
          <div class="timeline-item">
            <h3>Programming Hub Certifications</h3>
            <p>Completed 85+ certifications covering development, programming concepts, and software-related skills.</p>
          </div>

          <div class="timeline-item">
            <h3>Full-Stack Learning Journey</h3>
            <p>Ongoing study in web development, backend systems, mobile applications, and deployment practices.</p>
          </div>

          <div class="timeline-item">
            <h3>Practical Skill Development</h3>
            <p>Focused on applying knowledge through projects, experimentation, and continuous real-world practice.</p>
          </div>
        </div>
      </div>
    </section>

    <section id="contact">
      <div class="container">
        <div class="section-heading">
          <h2>Contact</h2>
          <p>
            Interested in collaboration, freelance work, or professional opportunities? Let’s connect.
          </p>
        </div>

        <div class="contact-box">
          <p>
            You can reach me through GitHub, email, or professional networks. Replace the placeholder links below with your real contact details.
          </p>

          <ul class="contact-list">
            <li>GitHub: <a href="https://github.com/moekyawaung-designer" target="_blank">github.com/moekyawaung-designer</a></li>
            <li>Email: <a href="mailto:your-email@example.com">your-email@example.com</a></li>
            <li>LinkedIn: <a href="#">Add your LinkedIn profile</a></li>
            <li>Portfolio: <a href="https://moekyawaung-designer.github.io" target="_blank">moekyawaung-designer.github.io</a></li>
          </ul>
        </div>
      </div>
    </section>
  </main>

  <footer>
    <div class="container">
      © 2025 Moe Kya Waung · Built with GitHub Pages
    </div>
  </footer>
</body>
</html>
