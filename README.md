<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Radh Shahmat · GitHub Profile</title>
  <!-- Font Awesome 6 (free) for icons -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css" />
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      background: #0d1117;
      display: flex;
      justify-content: center;
      padding: 2rem 1rem;
      font-family: 'Segoe UI', 'Inter', system-ui, -apple-system, sans-serif;
      line-height: 1.6;
      color: #e6edf3;
    }

    .github-md {
      max-width: 1000px;
      width: 100%;
      background: #161b22;
      border-radius: 32px;
      padding: 2.5rem 2.8rem;
      box-shadow: 0 20px 40px -12px rgba(0,0,0,0.8);
      border: 1px solid #30363d;
    }

    /* ----- banner ----- */
    .banner {
      background: linear-gradient(145deg, #1f2a3f, #0d1b2a);
      border-radius: 28px;
      padding: 1.8rem 2.2rem;
      margin-bottom: 2.2rem;
      display: flex;
      align-items: center;
      gap: 1rem;
      flex-wrap: wrap;
      border: 1px solid #30363d;
    }

    .banner i {
      font-size: 2.8rem;
      color: #58a6ff;
      opacity: 0.9;
      background: #0d1117;
      padding: 0.6rem 1rem;
      border-radius: 60px;
      border: 1px solid #30363d;
    }

    .banner-text {
      flex: 1;
      font-size: 1.2rem;
      font-weight: 400;
      color: #c9d1d9;
    }

    .banner-text strong {
      color: #f0f6fc;
      font-weight: 600;
    }

    .banner-text .badge {
      background: #21262d;
      padding: 0.2rem 0.8rem;
      border-radius: 40px;
      font-size: 0.8rem;
      color: #58a6ff;
      border: 1px solid #30363d;
      margin-left: 0.5rem;
    }

    /* ----- profile row (avatar + name + location/email) ----- */
    .profile-row {
      display: flex;
      align-items: center;
      gap: 1.8rem;
      flex-wrap: wrap;
      margin-bottom: 2rem;
      border-bottom: 1px solid #30363d;
      padding-bottom: 1.8rem;
    }

    .avatar-frame {
      width: 110px;
      height: 110px;
      border-radius: 50%;
      background: linear-gradient(135deg, #58a6ff, #1f6feb);
      padding: 3px;
      flex-shrink: 0;
      box-shadow: 0 0 0 1px #30363d;
    }

    .avatar {
      width: 100%;
      height: 100%;
      border-radius: 50%;
      background: #0d1117;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 3.2rem;
      font-weight: 600;
      color: #f0f6fc;
      letter-spacing: 0.04em;
      background-image: radial-gradient(circle at 30% 30%, #2d3a4d, #0d1117);
      border: 2px solid #161b22;
    }

    .name-title {
      flex: 1;
    }

    .name-title h1 {
      font-size: 2.4rem;
      font-weight: 700;
      letter-spacing: -0.02em;
      color: #f0f6fc;
      margin-bottom: 0.2rem;
    }

    .designation {
      font-size: 1.1rem;
      color: #8b949e;
      display: flex;
      align-items: center;
      gap: 0.3rem;
      flex-wrap: wrap;
    }

    .designation i {
      color: #58a6ff;
      font-size: 0.9rem;
    }

    .location-email {
      display: flex;
      flex-wrap: wrap;
      gap: 1.2rem 2rem;
      margin-top: 0.6rem;
      font-size: 0.95rem;
      color: #8b949e;
    }

    .location-email i {
      color: #58a6ff;
      width: 1.2rem;
    }

    .location-email a {
      color: #58a6ff;
      text-decoration: none;
      border-bottom: 1px dotted #30363d;
    }

    .location-email a:hover {
      color: #1f6feb;
      border-bottom: 1px solid #58a6ff;
    }

    /* ----- about + activity bullets ----- */
    .about-section {
      background: #0d1117;
      padding: 1.5rem 1.8rem;
      border-radius: 24px;
      margin-bottom: 2rem;
      border: 1px solid #30363d;
    }

    .about-section h2 {
      font-size: 1.5rem;
      font-weight: 600;
      color: #f0f6fc;
      margin-bottom: 0.8rem;
      display: flex;
      align-items: center;
      gap: 0.5rem;
    }

    .about-section h2 i {
      color: #58a6ff;
      font-size: 1.3rem;
    }

    .about-section p {
      color: #c9d1d9;
      margin-bottom: 1rem;
      font-size: 1rem;
    }

    .activity-list {
      list-style: none;
      display: flex;
      flex-wrap: wrap;
      gap: 0.8rem 1.8rem;
      margin-top: 0.5rem;
    }

    .activity-list li {
      display: flex;
      align-items: center;
      gap: 0.5rem;
      background: #161b22;
      padding: 0.3rem 1rem 0.3rem 0.8rem;
      border-radius: 40px;
      border: 1px solid #30363d;
      font-size: 0.95rem;
      color: #e6edf3;
    }

    .activity-list li i {
      color: #58a6ff;
      font-size: 0.9rem;
    }

    /* ----- skills (icon-based grid) ----- */
    .skills-section {
      margin: 2rem 0 2.2rem;
    }

    .skills-section h2 {
      font-size: 1.5rem;
      font-weight: 600;
      color: #f0f6fc;
      margin-bottom: 1.2rem;
      display: flex;
      align-items: center;
      gap: 0.5rem;
    }

    .skills-section h2 i {
      color: #58a6ff;
    }

    .skills-grid {
      display: flex;
      flex-wrap: wrap;
      gap: 1rem 1.8rem;
      background: #0d1117;
      padding: 1.5rem 1.8rem;
      border-radius: 28px;
      border: 1px solid #30363d;
    }

    .skill-item {
      display: flex;
      align-items: center;
      gap: 0.6rem;
      font-size: 1rem;
      background: #161b22;
      padding: 0.4rem 1.2rem 0.4rem 1rem;
      border-radius: 40px;
      border: 1px solid #30363d;
      color: #e6edf3;
    }

    .skill-item i {
      font-size: 1.4rem;
      width: 1.8rem;
      text-align: center;
      color: #58a6ff;
    }
    /* brand colors for some icons */
    .skill-item .fa-js { color: #f7df1e; }
    .skill-item .fa-react { color: #61dafb; }
    .skill-item .fa-node { color: #68a063; }
    .skill-item .fa-database { color: #00758f; }
    .skill-item .fa-python { color: #3776ab; }
    .skill-item .fa-git { color: #f05033; }
    .skill-item .fa-html5 { color: #e34f26; }
    .skill-item .fa-css3-alt { color: #1572b6; }

    /* ----- social links ----- */
    .social-links {
      display: flex;
      flex-wrap: wrap;
      gap: 1.2rem;
      margin: 1.8rem 0 2rem;
      background: #0d1117;
      padding: 1rem 1.8rem;
      border-radius: 40px;
      border: 1px solid #30363d;
      justify-content: center;
    }

    .social-links a {
      color: #8b949e;
      font-size: 1.6rem;
      transition: 0.2s;
      display: inline-flex;
      align-items: center;
      gap: 0.3rem;
    }

    .social-links a:hover {
      color: #58a6ff;
      transform: scale(1.05);
    }

    .social-links a span {
      font-size: 0.9rem;
      font-weight: 400;
      color: #8b949e;
    }

    /* ----- stats row (contrib, languages, streak) ----- */
    .stats-row {
      display: flex;
      flex-wrap: wrap;
      justify-content: space-around;
      gap: 1.5rem;
      background: #0d1117;
      padding: 1.2rem 1.5rem;
      border-radius: 28px;
      border: 1px solid #30363d;
      margin-bottom: 2.2rem;
    }

    .stat-item {
      display: flex;
      align-items: center;
      gap: 0.6rem;
      color: #c9d1d9;
      font-size: 0.95rem;
    }

    .stat-item i {
      color: #58a6ff;
      font-size: 1.4rem;
    }

    .stat-item strong {
      color: #f0f6fc;
      font-weight: 600;
      margin-right: 0.2rem;
    }

    /* ----- pinned repositories ----- */
    .pinned-header {
      font-size: 1.5rem;
      font-weight: 600;
      color: #f0f6fc;
      margin: 2.2rem 0 1.5rem;
      display: flex;
      align-items: center;
      gap: 0.5rem;
    }

    .pinned-header i {
      color: #58a6ff;
    }

    .repo-card {
      background: #0d1117;
      border: 1px solid #30363d;
      border-radius: 24px;
      padding: 1.8rem 2rem;
      margin-bottom: 2.2rem;
    }

    .repo-card h3 {
      font-size: 1.6rem;
      font-weight: 600;
      color: #58a6ff;
      margin-bottom: 0.3rem;
    }

    .repo-card h3 i {
      margin-right: 0.5rem;
      color: #8b949e;
      font-size: 1.3rem;
    }

    .repo-desc {
      color: #c9d1d9;
      font-size: 1rem;
      margin: 0.5rem 0 0.8rem;
    }

    .repo-tech {
      display: flex;
      flex-wrap: wrap;
      gap: 0.6rem 1.2rem;
      margin: 0.8rem 0 1rem;
    }

    .repo-tech span {
      background: #161b22;
      padding: 0.2rem 0.9rem;
      border-radius: 40px;
      font-size: 0.85rem;
      border: 1px solid #30363d;
      color: #8b949e;
      display: flex;
      align-items: center;
      gap: 0.3rem;
    }

    .repo-tech span i {
      color: #58a6ff;
      font-size: 0.8rem;
    }

    .repo-links {
      display: flex;
      flex-wrap: wrap;
      gap: 1rem 1.8rem;
      border-top: 1px solid #30363d;
      padding-top: 1rem;
      margin-top: 0.5rem;
    }

    .repo-links a {
      color: #58a6ff;
      text-decoration: none;
      font-size: 0.95rem;
      display: inline-flex;
      align-items: center;
      gap: 0.3rem;
    }

    .repo-links a:hover {
      color: #1f6feb;
      text-decoration: underline;
    }

    .repo-features {
      list-style: none;
      display: flex;
      flex-wrap: wrap;
      gap: 0.4rem 1.2rem;
      margin: 0.8rem 0;
    }

    .repo-features li {
      font-size: 0.95rem;
      color: #c9d1d9;
      display: flex;
      align-items: center;
      gap: 0.3rem;
    }

    .repo-features li i {
      color: #58a6ff;
      font-size: 0.8rem;
    }

    .repo-install {
      background: #161b22;
      border-radius: 16px;
      padding: 0.8rem 1.2rem;
      margin: 0.8rem 0;
      font-family: 'Fira Code', monospace;
      font-size: 0.9rem;
      color: #e6edf3;
      border: 1px solid #30363d;
      overflow-x: auto;
    }

    .repo-install i {
      color: #58a6ff;
      margin-right: 0.5rem;
    }

    .screenshot-placeholder {
      background: #161b22;
      border-radius: 16px;
      padding: 1rem 1.5rem;
      margin: 0.8rem 0;
      border: 1px solid #30363d;
      color: #8b949e;
      display: flex;
      align-items: center;
      gap: 0.8rem;
      font-size: 0.95rem;
    }

    .screenshot-placeholder i {
      font-size: 1.8rem;
      color: #58a6ff;
    }

    hr {
      border: 0;
      border-top: 1px solid #30363d;
      margin: 1.2rem 0;
    }

    /* responsive */
    @media (max-width: 700px) {
      .github-md { padding: 1.5rem; }
      .profile-row { flex-direction: column; align-items: flex-start; }
      .name-title h1 { font-size: 2rem; }
      .banner { flex-direction: column; align-items: flex-start; }
      .stats-row { flex-direction: column; align-items: flex-start; }
      .social-links { justify-content: flex-start; }
    }
  </style>
</head>
<body>
<div class="github-md">

  <!-- ====== BANNER ====== -->
  <div class="banner">
    <i class="fas fa-code"></i>
    <div class="banner-text">
      <strong>Radh Shahmat</strong> · full-stack explorer <span class="badge">#buildinpublic</span>
      <div style="font-size:0.9rem; margin-top:0.2rem; color:#8b949e;">
        <i class="fas fa-map-pin" style="color:#58a6ff;"></i> Dhaka, Bangladesh
      </div>
    </div>
  </div>

  <!-- ====== PROFILE ROW ====== -->
  <div class="profile-row">
    <div class="avatar-frame">
      <div class="avatar">RS</div>
    </div>
    <div class="name-title">
      <h1>Radh Shahmat</h1>
      <div class="designation">
        <i class="fas fa-bolt"></i> Software Engineer · MERN & Next.js
      </div>
      <div class="location-email">
        <span><i class="fas fa-map-marker-alt"></i> Dhaka, Bangladesh</span>
        <span><i class="fas fa-envelope"></i> <a href="mailto:radh.shahmat@example.com">radh.shahmat@example.com</a></span>
        <span><i class="fas fa-globe"></i> <a href="#">radh.dev</a></span>
      </div>
    </div>
  </div>

  <!-- ====== ABOUT ME ====== -->
  <div class="about-section">
    <h2><i class="fas fa-user-astronaut"></i> About me</h2>
    <p>Hi, I'm Radh — a passionate developer who loves crafting digital experiences. I blend clean design with robust logic, and I’m always curious about new tools. Currently diving deep into the JAMstack and cloud-native development.</p>
    <ul class="activity-list">
      <li><i class="fas fa-rocket"></i> Exploring Next.js 14 & App Router</li>
      <li><i class="fas fa-code-branch"></i> Working on a tourism platform</li>
      <li><i class="fas fa-cloud-sun"></i> Building open‑source utilities</li>
      <li><i class="fas fa-mug-saucer"></i> Coffee & clean code</li>
    </ul>
  </div>

  <!-- ====== SKILLS (icon-based) ====== -->
  <div class="skills-section">
    <h2><i class="fas fa-cogs"></i> Tech Stack</h2>
    <div class="skills-grid">
      <span class="skill-item"><i class="fab fa-js"></i> JavaScript</span>
      <span class="skill-item"><i class="fab fa-react"></i> React</span>
      <span class="skill-item"><i class="fab fa-node"></i> Node.js</span>
      <span class="skill-item"><i class="fas fa-database"></i> MongoDB</span>
      <span class="skill-item"><i class="fab fa-python"></i> Python</span>
      <span class="skill-item"><i class="fab fa-git"></i> Git</span>
      <span class="skill-item"><i class="fab fa-html5"></i> HTML5</span>
      <span class="skill-item"><i class="fab fa-css3-alt"></i> CSS3</span>
      <span class="skill-item"><i class="fas fa-cloud"></i> AWS</span>
      <span class="skill-item"><i class="fas fa-docker"></i> Docker</span>
    </div>
  </div>

  <!-- ====== SOCIAL LINKS ====== -->
  <div class="social-links">
    <a href="#"><i class="fab fa-github"></i> <span>github/radh</span></a>
    <a href="#"><i class="fab fa-linkedin-in"></i> <span>linkedin/radh</span></a>
    <a href="#"><i class="fab fa-twitter"></i> <span>@radh_dev</span></a>
    <a href="#"><i class="fab fa-dev"></i> <span>dev.to/radh</span></a>
    <a href="#"><i class="fas fa-envelope"></i> <span>email</span></a>
  </div>

  <!-- ====== STATS ====== -->
  <div class="stats-row">
    <div class="stat-item"><i class="fas fa-code-branch"></i> <strong>1.2k</strong> contributions</div>
    <div class="stat-item"><i class="fas fa-circle"></i> <strong>JS·TS·Python</strong> top languages</div>
    <div class="stat-item"><i class="fas fa-fire"></i> <strong>14</strong> day streak</div>
    <div class="stat-item"><i class="fas fa-star"></i> <strong>38</strong> stars earned</div>
  </div>

  <!-- ====== PINNED REPOSITORIES (2) ====== -->
  <div class="pinned-header">
    <i class="fas fa-thumbtack"></i> Pinned repositories
  </div>

  <!-- REPO 1: tourism-explorer -->
  <div class="repo-card">
    <h3><i class="fas fa-umbrella-beach"></i> tourism-explorer</h3>
    <div class="repo-desc">
      <i class="fas fa-globe" style="color:#58a6ff;"></i> 
      A modern tourism platform with interactive maps, itinerary builder, and real‑time weather. 
      <span style="color:#8b949e; font-size:0.9rem;"> · Live demo available</span>
    </div>
    <div class="repo-tech">
      <span><i class="fab fa-react"></i> React</span>
      <span><i class="fab fa-node"></i> Node.js</span>
      <span><i class="fas fa-database"></i> MongoDB</span>
      <span><i class="fas fa-cloud-sun"></i> Mapbox</span>
    </div>
    <!-- screenshot placeholder -->
    <div class="screenshot-placeholder">
      <i class="fas fa-image"></i> [ Screenshot: tourism dashboard with map & cards ]
    </div>
    <ul class="repo-features">
      <li><i class="fas fa-check-circle"></i> Interactive map with POIs</li>
      <li><i class="fas fa-check-circle"></i> User itinerary builder</li>
      <li><i class="fas fa-check-circle"></i> Weather & alerts</li>
      <li><i class="fas fa-check-circle"></i> Authentication & reviews</li>
    </ul>
    <div class="repo-install">
      <i class="fas fa-terminal"></i> git clone https://github.com/radh/tourism-explorer.git <br>
      <i class="fas fa-cog"></i> npm install && npm run dev
    </div>
    <div class="repo-links">
      <a href="#"><i class="fas fa-link"></i> Live demo</a>
      <a href="#"><i class="fab fa-github"></i> Repository</a>
      <a href="#"><i class="fas fa-book"></i> API docs</a>
    </div>
    <div style="margin-top:0.6rem; font-size:0.9rem; color:#8b949e;">
      <i class="fas fa-cubes"></i> Dependencies: express, mongoose, react-router, axios, mapbox-gl, jwt
    </div>
  </div>

  <!-- REPO 2: nextjs-starter-kit -->
  <div class="repo-card">
    <h3><i class="fas fa-rocket"></i> nextjs-starter-kit</h3>
    <div class="repo-desc">
      <i class="fas fa-code" style="color:#58a6ff;"></i> 
      Production‑ready Next.js 14 starter with authentication, i18n, and dark mode.
      <span style="color:#8b949e; font-size:0.9rem;"> · Tailwind + shadcn/ui</span>
    </div>
    <div class="repo-tech">
      <span><i class="fab fa-react"></i> Next.js 14</span>
      <span><i class="fab fa-node"></i> TypeScript</span>
      <span><i class="fas fa-palette"></i> Tailwind</span>
      <span><i class="fas fa-user-lock"></i> NextAuth</span>
    </div>
    <div class="screenshot-placeholder">
      <i class="fas fa-image"></i> [ Screenshot: clean dashboard with dark/light toggle ]
    </div>
    <ul class="repo-features">
      <li><i class="fas fa-check-circle"></i> App Router + Server Actions</li>
      <li><i class="fas fa-check-circle"></i> i18n (en/bn)</li>
      <li><i class="fas fa-check-circle"></i> Dark/light mode</li>
      <li><i class="fas fa-check-circle"></i> Prisma + PostgreSQL</li>
    </ul>
    <div class="repo-install">
      <i class="fas fa-terminal"></i> git clone https://github.com/radh/nextjs-starter-kit.git <br>
      <i class="fas fa-cog"></i> npm install && npm run dev
    </div>
    <div class="repo-links">
      <a href="#"><i class="fas fa-link"></i> Live demo</a>
      <a href="#"><i class="fab fa-github"></i> Repository</a>
      <a href="#"><i class="fas fa-file-alt"></i> Blog post</a>
    </div>
    <div style="margin-top:0.6rem; font-size:0.9rem; color:#8b949e;">
      <i class="fas fa-cubes"></i> Dependencies: next, react, prisma, next-auth, tailwind, i18next, shadcn/ui
    </div>
  </div>

  <hr />
  <div style="text-align:center; color:#8b949e; font-size:0.85rem; margin-top:1rem;">
    <i class="fas fa-code"></i> built with <i class="fas fa-heart" style="color:#f85149;"></i> · Radh Shahmat · 2026
  </div>
</div>
</body>
</html>
