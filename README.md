<!--<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Aaron Medrano Brenes — Data Analyst / Data Science / BI</title>
<style>
  :root {
    --bg: #0d1117;
    --surface: #161b22;
    --surface2: #1c2128;
    --border: #30363d;
    --text: #e6edf3;
    --text-dim: #8b949e;
    --accent: #58a6ff;
    --accent2: #3fb950;
    --accent3: #d2a8ff;
    --radius: 12px;
  }
  * { margin: 0; padding: 0; box-sizing: border-box; }
  body {
    background: var(--bg);
    color: var(--text);
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif;
    line-height: 1.6;
    max-width: 980px;
    margin: 0 auto;
    padding: 32px 20px 64px;
  }
  a { color: var(--accent); text-decoration: none; }
  a:hover { text-decoration: underline; }

  /* ── Hero ── */
  .hero {
    text-align: center;
    padding: 48px 24px 40px;
    background: linear-gradient(135deg, #161b22 0%, #0d1117 50%, #161b22 100%);
    border: 1px solid var(--border);
    border-radius: var(--radius);
    position: relative;
    overflow: hidden;
    margin-bottom: 32px;
  }
  .hero::before {
    content: "";
    position: absolute;
    top: -50%; left: -50%; width: 200%; height: 200%;
    background: radial-gradient(circle at 30% 40%, rgba(88,166,255,0.08) 0%, transparent 60%),
                radial-gradient(circle at 70% 60%, rgba(210,168,255,0.06) 0%, transparent 60%);
    pointer-events: none;
  }
  .hero h1 {
    font-size: 2.4rem;
    font-weight: 800;
    letter-spacing: -0.5px;
    background: linear-gradient(90deg, #58a6ff, #d2a8ff, #3fb950);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    position: relative;
  }
  .hero .tagline {
    font-size: 1.05rem; color: var(--text-dim);
    margin-top: 8px; position: relative;
  }
  .hero .meta { margin-top: 14px; font-size: 0.9rem; color: var(--text-dim); position: relative; }
  .hero .meta span { margin: 0 6px; }

  /* ── Sección títulos ── */
  .section-title {
    font-size: 1.25rem;
    font-weight: 700;
    margin: 40px 0 16px;
    padding-bottom: 8px;
    border-bottom: 1px solid var(--border);
    display: flex;
    align-items: center;
    gap: 8px;
  }
  .section-title .icon { font-size: 1.3rem; }

  /* ── Grid & Cards ── */
  .grid { display: grid; gap: 16px; }
  .grid-2 { grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); }
  .card {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: var(--radius);
    padding: 20px 22px;
    transition: border-color 0.2s, transform 0.15s;
  }
  .card:hover { border-color: var(--accent); transform: translateY(-2px); }
  .card h3 { font-size: 1rem; font-weight: 700; margin-bottom: 6px; color: var(--accent); }
  .card p { font-size: 0.9rem; color: var(--text-dim); margin-bottom: 10px; }
  .card .stack { display: flex; flex-wrap: wrap; gap: 6px; margin-top: 10px; }
  .card .stack code {
    background: var(--surface2);
    border: 1px solid var(--border);
    padding: 2px 8px; border-radius: 6px;
    font-size: 0.75rem; color: var(--text-dim);
    font-family: "SF Mono", "Fira Code", monospace;
  }

  /* ── Badges ── */
  .badges { display: flex; flex-wrap: wrap; gap: 6px; margin: 8px 0; }
  .badges img { height: 24px; }

  /* ── Stats rows ── */
  .stats-row {
    display: flex; flex-wrap: wrap; gap: 16px;
    justify-content: center; margin: 8px 0;
  }
  .stats-row img { max-width: 100%; }

  /* ── Pipeline ── */
  .pipeline {
    display: flex; flex-wrap: wrap; align-items: center; justify-content: center;
    gap: 6px; padding: 18px 12px;
    background: var(--surface); border: 1px solid var(--border);
    border-radius: var(--radius); font-size: 0.85rem;
    font-weight: 600; color: var(--text-dim);
  }
  .pipeline .step {
    background: var(--surface2); border: 1px solid var(--border);
    border-radius: 20px; padding: 5px 14px; white-space: nowrap;
  }
  .pipeline .arrow { color: var(--accent); font-size: 1rem; }

  /* ── Highlight ── */
  .highlight {
    background: linear-gradient(135deg, rgba(88,166,255,0.08), rgba(210,168,255,0.06));
    border: 1px solid rgba(88,166,255,0.25);
    border-radius: var(--radius);
    padding: 22px 24px; margin: 16px 0;
  }
  .highlight p { font-size: 0.95rem; color: var(--text-dim); margin: 0; }

  /* ── Footer ── */
  .footer {
    text-align: center; margin-top: 48px; padding-top: 24px;
    border-top: 1px solid var(--border);
    font-size: 0.85rem; color: var(--text-dim);
  }
  .footer a { color: var(--accent); }

  @media (max-width: 600px) {
    .hero h1 { font-size: 1.6rem; }
    .pipeline { font-size: 0.75rem; }
    .pipeline .step { padding: 4px 10px; }
  }
</style>
</head>
<body>

<!-- ═══════════════════════════════════════════════
     HERO
     ═══════════════════════════════════════════════ -->
<div class="hero">
  <h1>Aaron Medrano Brenes</h1>
  <p class="tagline">Data Analyst · Data Science · Business Intelligence</p>
  <p class="meta">
    <span>📍 San Jose, Costa Rica</span> ·
    <span>📧 <a href="mailto:damedrab24@outlook.com">damedrab24@outlook.com</a></span> ·
    <span>📱 +506 7252-9689</span>
  </p>
  <p class="meta" style="margin-top:10px;">
    <a href="https://github.com/AaronAllStar">GitHub</a> ·
    <a href="https://www.linkedin.com/in/aaron-medrano-brenes">LinkedIn</a>
  </p>
</div>

<!-- ═══════════════════════════════════════════════
     PROFILE
     ═══════════════════════════════════════════════ -->
<h2 class="section-title"><span class="icon">👤</span> Profile</h2>
<p style="color:var(--text-dim); font-size:0.95rem;">
  Data Science student focused on <strong style="color:var(--text);">Data Analytics, Business Intelligence</strong> and
  <strong style="color:var(--text);">data-driven software solutions</strong>. I build reproducible analytical
  workflows that connect business questions with data preparation, statistical modeling, quantitative metrics,
  visualization and decision support. My GitHub portfolio demonstrates hands-on work across financial risk,
  business analytics, quantitative systems, document analytics and full-stack data applications.
</p>

<!-- ═══════════════════════════════════════════════
     TECH STACK
     ═══════════════════════════════════════════════ -->
<h2 class="section-title"><span class="icon">🧰</span> Tech Stack</h2>

<p style="font-size:0.85rem; color:var(--text-dim); margin-bottom:6px;"><strong style="color:var(--text);">Languages</strong></p>
<div class="badges">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white" alt="Rust">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript">
  <img src="https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white" alt="SQL">
</div>

<p style="font-size:0.85rem; color:var(--text-dim); margin:10px 0 6px;"><strong style="color:var(--text);">Data &amp; Analytics</strong></p>
<div class="badges">
  <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" alt="Pandas">
  <img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white" alt="NumPy">
  <img src="https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white" alt="Jupyter">
  <img src="https://img.shields.io/badge/SciPy-8CAAE6?style=for-the-badge&logo=scipy&logoColor=white" alt="SciPy">
  <img src="https://img.shields.io/badge/Statsmodels-4B0082?style=for-the-badge&logo=python&logoColor=white" alt="Statsmodels">
</div>

<p style="font-size:0.85rem; color:var(--text-dim); margin:10px 0 6px;"><strong style="color:var(--text);">Databases</strong></p>
<div class="badges">
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL">
  <img src="https://img.shields.io/badge/SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white" alt="SQLite">
  <img src="https://img.shields.io/badge/pgvector-336791?style=for-the-badge&logo=postgresql&logoColor=white" alt="pgvector">
</div>

<p style="font-size:0.85rem; color:var(--text-dim); margin:10px 0 6px;"><strong style="color:var(--text);">Engineering &amp; Tools</strong></p>
<div class="badges">
  <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" alt="FastAPI">
  <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" alt="Node.js">
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker">
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" alt="Git">
  <img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white" alt="Redis">
  <img src="https://img.shields.io/badge/Celery-37814A?style=for-the-badge&logo=celery&logoColor=white" alt="Celery">
</div>

<!-- ═══════════════════════════════════════════════
     GITHUB STATS (Dinámicas y en tiempo real)
     ═══════════════════════════════════════════════ -->
<h2 class="section-title"><span class="icon">📊</span> GitHub Stats &amp; Activity</h2>

<!-- Tarjetas de GitCard Studio -->
<div class="stats-row">
  <img src="https://gitcard-studio.creativecode.com.co/api/stats?username=AaronAllStar&theme=dark&locale=en" alt="GitHub Stats" height="170">
  <img src="https://gitcard-studio.creativecode.com.co/api/languages?username=AaronAllStar&theme=tokyonight&locale=en" alt="Top Languages" height="170">
</div>
<div class="stats-row">
  <img src="https://gitcard-studio.creativecode.com.co/api/commit-activity?username=AaronAllStar&theme=neon&locale=en" alt="Commit Activity" height="170">
  <img src="https://neofetch-profile.vercel.app/api?username=AaronAllStar&theme=github-dark" alt="Neofetch Stats" height="170">
</div>

<!-- 3D Contributions & Activity Graph -->
<div style="text-align: center; margin: 24px 0;">
  <img src="https://github3d-api-production.up.railway.app/contributions/AaronAllStar/image.svg" alt="3D Contributions" style="max-width: 100%; border-radius: var(--radius);">
</div>
<div style="text-align: center; margin: 24px 0;">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=AaronAllStar&theme=github-dark&bg_color=0d1117&color=58a6ff&line=3fb950&point=d2a8ff" alt="Activity Graph" style="max-width: 100%; border-radius: var(--radius);">
</div>

<!-- Contador de Visitas -->
<div style="text-align: center; margin: 16px 0;">
  <img src="https://komarev.com/ghpvc/?username=AaronAllStar&style=for-the-badge&color=58a6ff" alt="Profile Views">
</div>

<!-- ═══════════════════════════════════════════════
     FEATURED PROJECTS
     ═══════════════════════════════════════════════ -->
<h2 class="section-title"><span class="icon">🚀</span> Featured Projects</h2>

<div class="grid grid-2">

  <!-- Café Cordillera -->
  <div class="card">
    <h3>☕ Café Cordillera Analytics</h3>
    <p><strong style="color:var(--text);">Business Analytics &amp; Statistical Consulting</strong></p>
    <p>End-to-end analytics product for a coffee-chain business combining statistical analysis with executive data
       storytelling. Implemented <strong>10 analytical metrics</strong> — from descriptive statistics to multiple
       linear regression, Bayesian analysis and Poisson modeling. Produced a reproducible Jupyter analysis,
       interactive standalone dashboard and consulting-style PDF.</p>
    <div class="stack">
      <code>Python</code><code>Pandas</code><code>SciPy</code><code>Statsmodels</code>
      <code>Jupyter</code><code>Chart.js</code><code>FastAPI</code>
    </div>
  </div>

  <!-- Credit Risk -->
  <div class="card">
    <h3>🏦 Credit Risk Scoring Engine</h3>
    <p><strong style="color:var(--text);">Quantitative Risk Analytics</strong></p>
    <p>Production-oriented credit-risk scoring engine using mathematically explicit classification models and a
       PostgreSQL analytical layer. Implemented <strong>L2-regularized logistic regression</strong> with class
       weighting for a severely imbalanced default problem, plus Gaussian Naive Bayes. Documented model assumptions,
       objective functions, computational complexity and evaluation methodology.</p>
    <div class="stack">
      <code>Rust</code><code>PostgreSQL</code><code>Logistic Regression</code>
      <code>Naive Bayes</code><code>Statistics</code>
    </div>
  </div>

  <!-- EdgeArena -->
  <div class="card">
    <h3>📈 EdgeArena</h3>
    <p><strong style="color:var(--text);">Quantitative Trading Analytics Platform</strong></p>
    <p>Quantitative platform for building, testing and comparing trading strategies against historical market data.
       Implemented <strong>parallelized backtesting infrastructure</strong> and quantitative performance analytics
       including Sharpe ratio and drawdown. Combined data processing, asynchronous jobs, APIs, relational storage
       and interactive charts into a production-style analytics system.</p>
    <div class="stack">
      <code>Python</code><code>Pandas</code><code>NumPy</code><code>FastAPI</code>
      <code>PostgreSQL</code><code>Redis</code><code>Celery</code><code>Next.js</code>
    </div>
  </div>

  <!-- Enterprise RAG -->
  <div class="card">
    <h3>📄 Enterprise RAG &amp; Document Analytics</h3>
    <p><strong style="color:var(--text);">Document Intelligence &amp; Vector Search</strong></p>
    <p>Document analytics pipeline for PDFs, Excel files and images, including structured extraction, OCR and
       tabular processing. Implemented <strong>vector embeddings</strong> and cosine-similarity search in
       PostgreSQL/pgvector to retrieve relevant document evidence. Generated structured analytical reports with
       executive summaries, key metrics, technical findings, conclusions and source traceability.</p>
    <div class="stack">
      <code>Python</code><code>FastAPI</code><code>PostgreSQL</code><code>pgvector</code>
      <code>Pandas</code><code>OCR</code><code>Gemini</code><code>Next.js</code>
    </div>
  </div>

  <!-- OpenIntel -->
  <div class="card">
    <h3>🕵️ OpenIntel</h3>
    <p><strong style="color:var(--text);">Unified OSINT Intelligence Platform</strong></p>
    <p>Self-hosted OSINT investigation cockpit that orchestrates <strong>27 specialized reconnaissance engines</strong>
       behind a real-time cyberpunk-inspired dashboard. Normalizes, deduplicates and correlates findings into an
       interactive graph with evidence provenance tracking. Features live SSE streaming, 5 multi-modal search spaces,
       granular engine selection and single-container Docker packaging serving React/Tailwind + FastAPI on port 8000.</p>
    <div class="stack">
      <code>Python</code><code>FastAPI</code><code>React</code><code>Tailwind</code>
      <code>Docker</code><code>SSE</code><code>OSINT</code>
    </div>
  </div>

  <!-- Noty Mejorado -->
  <div class="card">
    <h3>🔐 Noty Mejorado</h3>
    <p><strong style="color:var(--text);">REST Data Application</strong></p>
    <p>Full-stack application demonstrating relational data persistence, REST API design and secure user-specific
       data access. Implemented authentication with <strong>JWT</strong>, password hashing with <strong>bcrypt</strong>
       and protected CRUD operations for user-owned records. Demonstrates the software-engineering foundation used to
       turn analytical workflows into maintainable data applications.</p>
    <div class="stack">
      <code>Node.js</code><code>Express</code><code>SQLite</code>
      <code>REST API</code><code>JWT</code><code>JavaScript</code>
    </div>
  </div>

</div>

<!-- ═══════════════════════════════════════════════
     PROFESSIONAL APPROACH
     ═══════════════════════════════════════════════ -->
<h2 class="section-title"><span class="icon">🎯</span> Professional Approach</h2>

<div class="pipeline">
  <span class="step">Business Problem</span><span class="arrow">→</span>
  <span class="step">Data Requirements</span><span class="arrow">→</span>
  <span class="step">Solution Alternatives</span><span class="arrow">→</span>
  <span class="step">Data/Model Design</span><span class="arrow">→</span>
  <span class="step">Implementation</span><span class="arrow">→</span>
  <span class="step">Analysis &amp; Validation</span><span class="arrow">→</span>
  <span class="step">Visualization</span><span class="arrow">→</span>
  <span class="step">Stakeholder Feedback</span><span class="arrow">→</span>
  <span class="step">Final Delivery</span>
</div>

<div class="highlight">
  <p>
    <strong style="color:var(--text);">💡 Evidence-driven portfolio.</strong>
    Each featured project links directly to a public GitHub repository where recruiters can inspect documentation,
    methodology, architecture and implementation. I don't just write code — I build reproducible analytical systems
    that solve real business problems.
  </p>
</div>

<!-- ═══════════════════════════════════════════════
     FOOTER
     ═══════════════════════════════════════════════ -->
<div class="footer">
  <p>
    <a href="https://github.com/AaronAllStar">GitHub</a> ·
    <a href="https://www.linkedin.com/in/aaron-medrano-brenes">LinkedIn</a> ·
    <a href="mailto:damedrab24@outlook.com">damedrab24@outlook.com</a>
  </p>
  <p style="margin-top:6px;">Building data systems that actually work. 🇨🇷</p>
</div>

</body>
</html>
