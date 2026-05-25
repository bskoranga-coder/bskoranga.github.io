<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Prof. Bipin Singh Koranga | Neutrino Physicist</title>
  <link href="https://fonts.googleapis.com/css2?family=EB+Garamond:ital,wght@0,400;0,500;0,600;1,400;1,500&family=DM+Mono:wght@300;400;500&family=Cormorant+Garamond:ital,wght@0,300;0,400;1,300;1,400&display=swap" rel="stylesheet">
  <style>
    :root {
      --bg: #faf8f4;
      --surface: #f2ede4;
      --ink: #1a1714;
      --ink-soft: #4a4540;
      --ink-muted: #8a8078;
      --accent: #8b1a1a;
      --accent-warm: #c0703a;
      --accent-light: #e8d5c0;
      --border: #d8cfc0;
      --mono: 'DM Mono', monospace;
      --serif: 'EB Garamond', serif;
      --display: 'Cormorant Garamond', serif;
    }

    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
    html { scroll-behavior: smooth; }
    body {
      background: var(--bg);
      color: var(--ink);
      font-family: var(--serif);
      font-size: 17px;
      line-height: 1.75;
      min-height: 100vh;
    }

    .page {
      max-width: 860px;
      margin: 0 auto;
      padding: 0 2rem 6rem;
    }

    header {
      display: grid;
      grid-template-columns: 1fr auto;
      gap: 2.5rem;
      align-items: start;
      padding: 4rem 0 2.5rem;
      border-bottom: 1px solid var(--border);
    }

    .header-text h1 {
      font-family: var(--display);
      font-size: 2.9rem;
      font-weight: 300;
      letter-spacing: 0.01em;
      line-height: 1.15;
    }

    .header-text .title-line {
      font-family: var(--mono);
      font-size: 0.72rem;
      letter-spacing: 0.14em;
      color: var(--accent);
      text-transform: uppercase;
      margin-top: 0.6rem;
      margin-bottom: 0.4rem;
    }

    .header-text .institution {
      font-size: 1rem;
      color: var(--ink-soft);
      font-style: italic;
    }

    .header-photo img {
      width: 165px;
      height: 165px;
      object-fit: cover;
      border-radius: 4px;
      border: 1px solid var(--border);
      display: block;
    }

    .photo-placeholder {
      width: 165px;
      height: 165px;
      background: var(--surface);
      border: 1px solid var(--border);
      border-radius: 4px;
      display: flex;
      align-items: center;
      justify-content: center;
      color: var(--ink-muted);
      font-family: var(--mono);
      font-size: 0.65rem;
      letter-spacing: 0.08em;
      text-align: center;
      padding: 1rem;
    }

    nav {
      display: flex;
      gap: 0;
      padding: 1.1rem 0;
      border-bottom: 1px solid var(--border);
      flex-wrap: wrap;
    }

    nav a {
      font-family: var(--mono);
      font-size: 0.72rem;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      color: var(--ink-soft);
      text-decoration: none;
      padding: 0.3rem 1.1rem 0.3rem 0;
      transition: color 0.2s;
    }

    nav a:not(:last-child)::after {
      content: '/';
      margin-left: 1.1rem;
      color: var(--border);
    }

    nav a:hover { color: var(--accent); }

    .opportunity-banner {
      margin: 2.2rem 0;
      background: var(--surface);
      border-left: 3px solid var(--accent);
      padding: 1.2rem 1.5rem;
      border-radius: 0 4px 4px 0;
    }

    .opportunity-banner p {
      font-size: 0.96rem;
      color: var(--ink-soft);
      line-height: 1.7;
    }

    .opportunity-banner strong { color: var(--accent); }

    .opportunity-banner .email-link {
      display: inline-block;
      margin-top: 0.6rem;
      font-family: var(--mono);
      font-size: 0.75rem;
      color: var(--accent-warm);
      text-decoration: none;
      letter-spacing: 0.04em;
    }

    .opportunity-banner .email-link:hover { text-decoration: underline; }

    section {
      margin-top: 3rem;
      padding-top: 3rem;
      border-top: 1px solid var(--border);
    }

    .section-label {
      font-family: var(--mono);
      font-size: 0.65rem;
      letter-spacing: 0.18em;
      text-transform: uppercase;
      color: var(--ink-muted);
      margin-bottom: 1.4rem;
    }

    h2 {
      font-family: var(--display);
      font-size: 1.95rem;
      font-weight: 300;
      color: var(--ink);
      margin-bottom: 1.4rem;
      line-height: 1.2;
    }

    .edu-block {
      padding: 1.2rem 0;
      border-bottom: 1px dashed var(--border);
    }

    .edu-block:last-child { border-bottom: none; }

    .edu-degree { font-weight: 600; font-size: 1rem; }

    .edu-inst {
      font-style: italic;
      color: var(--ink-soft);
      margin-top: 0.1rem;
    }

    .edu-meta {
      font-family: var(--mono);
      font-size: 0.7rem;
      color: var(--ink-muted);
      letter-spacing: 0.06em;
      margin-top: 0.3rem;
    }

    .edu-thesis {
      margin-top: 0.5rem;
      font-size: 0.92rem;
      color: var(--ink-soft);
      font-style: italic;
    }

    .interests-cloud {
      display: flex;
      flex-wrap: wrap;
      gap: 0.5rem 0.7rem;
      margin-top: 0.5rem;
    }

    .interest-tag {
      font-size: 0.83rem;
      background: var(--surface);
      border: 1px solid var(--border);
      color: var(--ink-soft);
      padding: 0.3rem 0.75rem;
      border-radius: 2px;
    }

    .pub-count {
      font-family: var(--mono);
      font-size: 0.72rem;
      color: var(--accent-warm);
      letter-spacing: 0.08em;
      margin-bottom: 1.2rem;
    }

    .pub-list {
      list-style: none;
      display: flex;
      flex-direction: column;
      gap: 0.8rem;
    }

    .pub-list li {
      padding-left: 1.2rem;
      position: relative;
      font-size: 0.95rem;
    }

    .pub-list li::before {
      content: '—';
      position: absolute;
      left: 0;
      color: var(--accent);
    }

    .pub-list a {
      color: var(--ink);
      text-decoration: underline;
      text-decoration-color: var(--accent-light);
      text-underline-offset: 3px;
      transition: color 0.2s;
    }

    .pub-list a:hover { color: var(--accent); }

    .profiles-grid {
      display: flex;
      flex-wrap: wrap;
      gap: 0.7rem;
      margin-top: 0.5rem;
    }

    .profile-link {
      font-family: var(--mono);
      font-size: 0.71rem;
      letter-spacing: 0.07em;
      text-transform: uppercase;
      color: var(--ink-soft);
      text-decoration: none;
      border: 1px solid var(--border);
      padding: 0.4rem 0.9rem;
      border-radius: 2px;
      transition: all 0.2s;
    }

    .profile-link:hover {
      background: var(--accent);
      color: white;
      border-color: var(--accent);
    }

    .timeline { display: flex; flex-direction: column; gap: 0; }

    .timeline-item {
      display: grid;
      grid-template-columns: 180px 1fr;
      gap: 1.2rem;
      padding: 0.8rem 0;
      border-bottom: 1px dashed var(--border);
      align-items: start;
    }

    .timeline-item:last-child { border-bottom: none; }

    .timeline-year {
      font-family: var(--mono);
      font-size: 0.68rem;
      color: var(--ink-muted);
      letter-spacing: 0.06em;
      padding-top: 0.15rem;
    }

    .timeline-role { font-size: 0.94rem; line-height: 1.5; }

    .timeline-place {
      font-style: italic;
      color: var(--ink-soft);
      font-size: 0.88rem;
    }

    .award-list {
      list-style: none;
      display: flex;
      flex-direction: column;
      gap: 0.9rem;
    }

    .award-list li {
      padding: 0.9rem 1.1rem;
      background: var(--surface);
      border-radius: 3px;
      border-left: 2px solid var(--accent-warm);
      font-size: 0.92rem;
    }

    .award-year {
      font-family: var(--mono);
      font-size: 0.65rem;
      color: var(--ink-muted);
      letter-spacing: 0.08em;
      display: block;
      margin-top: 0.2rem;
    }

    .books-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
      gap: 1rem;
      margin-top: 0.5rem;
    }

    .book-card {
      border: 1px solid var(--border);
      background: var(--surface);
      padding: 1rem 1.1rem;
      border-radius: 3px;
      font-size: 0.88rem;
      transition: border-color 0.2s;
    }

    .book-card:hover { border-color: var(--accent); }

    .book-card a {
      color: var(--ink);
      text-decoration: none;
      font-style: italic;
      font-weight: 500;
    }

    .book-card a:hover { color: var(--accent); }

    .visit-list {
      list-style: none;
      display: flex;
      flex-direction: column;
      gap: 0.6rem;
    }

    .visit-list li {
      font-size: 0.93rem;
      padding-left: 1.2rem;
      position: relative;
      color: var(--ink-soft);
    }

    .visit-list li::before {
      content: '◆';
      position: absolute;
      left: 0;
      font-size: 0.4rem;
      color: var(--accent-warm);
      top: 0.55rem;
    }

    .students-intro {
      font-size: 0.95rem;
      color: var(--ink-soft);
      margin-bottom: 2rem;
      font-style: italic;
    }

    .student-card {
      margin-bottom: 1.8rem;
      padding: 1.4rem 1.6rem;
      background: var(--surface);
      border: 1px solid var(--border);
      border-radius: 4px;
      position: relative;
      overflow: hidden;
    }

    .student-card::before {
      content: '';
      position: absolute;
      top: 0; left: 0;
      width: 3px;
      height: 100%;
      background: var(--accent);
    }

    .student-header {
      display: flex;
      justify-content: space-between;
      align-items: baseline;
      flex-wrap: wrap;
      gap: 0.4rem;
      margin-bottom: 0.9rem;
    }

    .student-name {
      font-family: var(--display);
      font-size: 1.25rem;
      font-weight: 400;
    }

    .student-badge {
      font-family: var(--mono);
      font-size: 0.63rem;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      color: var(--accent-warm);
      background: var(--accent-light);
      padding: 0.2rem 0.6rem;
      border-radius: 2px;
    }

    .student-works {
      list-style: none;
      display: flex;
      flex-direction: column;
      gap: 0.5rem;
    }

    .student-works li {
      font-size: 0.88rem;
      padding-left: 1rem;
      position: relative;
      color: var(--ink-soft);
      line-height: 1.5;
    }

    .student-works li::before {
      content: '↳';
      position: absolute;
      left: 0;
      color: var(--accent);
    }

    .student-works a {
      color: var(--ink-soft);
      text-decoration: underline;
      text-decoration-color: var(--border);
      text-underline-offset: 2px;
      transition: color 0.2s;
    }

    .student-works a:hover { color: var(--accent); }

    .work-type-badge {
      font-family: var(--mono);
      font-size: 0.6rem;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      color: var(--ink-muted);
      background: var(--bg);
      border: 1px solid var(--border);
      padding: 0.1rem 0.4rem;
      border-radius: 2px;
      margin-left: 0.4rem;
      vertical-align: middle;
    }

    footer {
      margin-top: 5rem;
      padding-top: 2rem;
      border-top: 1px solid var(--border);
      font-family: var(--mono);
      font-size: 0.65rem;
      letter-spacing: 0.1em;
      color: var(--ink-muted);
      text-align: center;
      text-transform: uppercase;
    }

    @media (max-width: 620px) {
      header { grid-template-columns: 1fr; }
      .header-photo { display: none; }
      .timeline-item { grid-template-columns: 1fr; }
    }
  </style>
</head>
<body>
<div class="page">

  <header>
    <div class="header-text">
      <div class="title-line">Neutrino Physicist · Professor of Physics</div>
      <h1>Bipin Singh<br>Koranga</h1>
      <div class="institution">Kirori Mal College, University of Delhi</div>
    </div>
    <div class="header-photo">
      <div class="photo-placeholder">Photo<br>assets/img/<br>Bipin_pfp.jpeg</div>
      <!-- Replace above div with: <img src="assets/img/Bipin_pfp.jpeg" alt="Prof. Bipin Singh Koranga"> -->
    </div>
  </header>

  <nav>
    <a href="#education">Education</a>
    <a href="#research">Research</a>
    <a href="#publications">Publications</a>
    <a href="#experience">Experience</a>
    <a href="#books">Books</a>
    <a href="#students">Students</a>
    <a href="mailto:bskoranga@kmc.du.ac.in">Email</a>
  </nav>

  <div class="opportunity-banner">
    <p>I welcome motivated students interested in research and seeking internships in <strong>High Energy Physics</strong> or <strong>Neutrino Physics</strong>. Students with strong curiosity and commitment to theoretical or phenomenological work are encouraged to get in touch.</p>
    <a href="mailto:bskoranga@kmc.du.ac.in" class="email-link">📧 bskoranga@kmc.du.ac.in</a>
  </div>

  <section id="education">
    <div class="section-label">Academic Background</div>
    <h2>Education</h2>
    <div class="edu-block">
      <div class="edu-degree">Ph.D. in Physics</div>
      <div class="edu-inst">Indian Institute of Technology (IIT) Bombay</div>
      <div class="edu-meta">Completed 2007 · CGPA 8.8 / 10 · Supervisor: S. Uma Sankar</div>
      <div class="edu-thesis">Thesis: Studies in Neutrino Masses and Mixings</div>
    </div>
  </section>

  <section id="research">
    <div class="section-label">Focus Areas</div>
    <h2>Research Interests</h2>
    <div class="interests-cloud">
      <span class="interest-tag">Neutrino Physics</span>
      <span class="interest-tag">Nuclear Physics</span>
      <span class="interest-tag">Cosmology</span>
      <span class="interest-tag">CP Violation in Neutrino Oscillations</span>
      <span class="interest-tag">Quantum Field Theory</span>
      <span class="interest-tag">High Energy Particle Physics</span>
      <span class="interest-tag">Mathematical Physics</span>
      <span class="interest-tag">Dark Matter Studies</span>
      <span class="interest-tag">Relativity & Astroparticle Physics</span>
      <span class="interest-tag">Quantum Information Theory</span>
    </div>
  </section>

  <section id="publications">
    <div class="section-label">Scholarly Output</div>
    <h2>Publications</h2>
    <div class="pub-count">60+ research papers in international journals</div>
    <ul class="pub-list">
      <li><a href="https://journals.aps.org/prd/accepted/10.1103/8r1c-knd2" target="_blank">Earth-density effects in long baseline neutrino experiments</a></li>
      <li><a href="https://doi.org/10.1016/j.physletb.2008.02.070" target="_blank">Deviation from bimaximality due to Planck scale effects</a></li>
      <li><a href="http://fizika.hfd.hr/fizika_b/bv09/b18p219.pdf" target="_blank">Possible CPT violation from Planck scale effects</a></li>
      <li><a href="https://doi.org/10.1016/j.nuclphysb.2026.117373" target="_blank">Modified entanglement patterns in two-flavor neutrinos from quantum-gravity interactions</a></li>
      <li><a href="https://doi.org/10.1142/S021974992540009X" target="_blank">Two Flavour Neutrino Oscillation in Matter and Quantum Entanglement</a></li>
    </ul>

    <div class="section-label" style="margin-top:2rem;">Research Profiles</div>
    <div class="profiles-grid">
      <a class="profile-link" href="https://www.researchgate.net/profile/Bipin-Singh-Koranga" target="_blank">ResearchGate</a>
      <a class="profile-link" href="https://scholar.google.co.in/citations?user=Zw-OC8kAAAAJ" target="_blank">Google Scholar</a>
      <a class="profile-link" href="https://www.linkedin.com/in/prof-dr-bipin-singh-koranga-22496157/" target="_blank">LinkedIn</a>
      <a class="profile-link" href="https://inspirehep.net/authors/1039975?ui-citation-summary=true" target="_blank">Inspire-HEP</a>
    </div>
  </section>

  <section id="experience">
    <div class="section-label">Career</div>
    <h2>Professional Experience</h2>
    <div class="timeline">
      <div class="timeline-item">
        <div class="timeline-year">Nov 2022 — Present</div>
        <div>
          <div class="timeline-role">Professor, Department of Physics</div>
          <div class="timeline-place">Kirori Mal College, University of Delhi</div>
        </div>
      </div>
      <div class="timeline-item">
        <div class="timeline-year">2019 — 2022</div>
        <div>
          <div class="timeline-role">Associate Professor, Department of Physics</div>
          <div class="timeline-place">Kirori Mal College, University of Delhi</div>
        </div>
      </div>
      <div class="timeline-item">
        <div class="timeline-year">2007 — 2019</div>
        <div>
          <div class="timeline-role">Assistant Professor, Department of Physics</div>
          <div class="timeline-place">Kirori Mal College, University of Delhi</div>
        </div>
      </div>
      <div class="timeline-item">
        <div class="timeline-year">2006 — 2007</div>
        <div>
          <div class="timeline-role">Postdoctoral Fellow — INO Simulation</div>
          <div class="timeline-place">TIFR and IIT Bombay</div>
        </div>
      </div>
      <div class="timeline-item">
        <div class="timeline-year">2006</div>
        <div>
          <div class="timeline-role">Postdoctoral Research — Magnetized Iron Neutrino Detector</div>
          <div class="timeline-place">Studies of Physics with MIND</div>
        </div>
      </div>
      <div class="timeline-item">
        <div class="timeline-year">2001 — 2006</div>
        <div>
          <div class="timeline-role">Teaching and Research Assistant</div>
          <div class="timeline-place">Department of Physics, IIT Bombay</div>
        </div>
      </div>
    </div>
  </section>

  <section id="awards">
    <div class="section-label">Honors</div>
    <h2>Awards & Distinctions</h2>
    <ul class="award-list">
      <li>
        <strong>Junior Merit Scholarship (Ekikrit Chhatravritti)</strong>
        <span class="award-year">1989 – 1993 · Awarded during 9th–12th standard</span>
      </li>
      <li>
        <strong>Graduation Merit Scholarship</strong>
        <span class="award-year">1995 – 1998 · During B.Sc. and M.Sc.</span>
      </li>
      <li>
        <strong>GATE Qualification</strong>
        <span class="award-year">2000 and 2001 · All India graduate aptitude examination organized by the IITs</span>
      </li>
      <li>
        <strong>GEST and NET Qualification</strong>
        <span class="award-year">1999 – 2001</span>
      </li>
    </ul>
  </section>

  <section id="visits">
    <div class="section-label">International</div>
    <h2>Foreign Visits</h2>
    <ul class="visit-list">
      <li>Workshop Towards Neutrino Technologies — ICTP, Trieste, Italy <span style="font-family:var(--mono);font-size:0.7rem;color:var(--ink-muted)">(July 2009)</span></li>
      <li>Workshop on Recent Developments in Astronuclear and Astroparticle Physics — ICTP, Trieste, Italy <span style="font-family:var(--mono);font-size:0.7rem;color:var(--ink-muted)">(November 2012)</span></li>
      <li>Summer School on Particle Physics — ICTP Trieste, Italy <span style="font-family:var(--mono);font-size:0.7rem;color:var(--ink-muted)">(June 2004)</span></li>
    </ul>
  </section>

  <section id="books">
    <div class="section-label">Authored Works</div>
    <h2>Books Written</h2>
    <div class="books-grid">
      <div class="book-card"><a href="https://www.flipkart.com/introduction-tensor-analysis/p/itm65543d7850873" target="_blank">An Introduction of Tensor Analysis</a></div>
      <div class="book-card"><a href="https://www.amazon.in/Special-Functions-Their-Application-Koranga/dp/8770042764/" target="_blank">Special Functions and Its Application</a></div>
      <div class="book-card"><a href="https://www.amazon.com/Introduction-Fluid-Dynamics-Ratindra-Gautam/dp/6205492520" target="_blank">An Introduction of Fluid Dynamics</a></div>
      <div class="book-card"><a href="https://www.amazon.com/LAGRANGIAN-HAMILTONIAN-DYNAMICS-Bipin-Koranga/dp/6206844331" target="_blank">Lagrangian and Hamiltonian Dynamics</a></div>
      <div class="book-card"><a href="https://www.amazon.in/Modern-Physics-Applications-Undergraduate-Postgraduate/dp/8195705456/" target="_blank">Modern Physics: Basic Concepts and Applications</a></div>
    </div>
  </section>

  <section id="students">
    <div class="section-label">Mentorship</div>
    <h2>Current Research Students</h2>
    <p class="students-intro">The following students are currently working under the supervision of Prof. Bipin Singh Koranga.</p>

    <div class="student-card">
      <div class="student-header">
        <div class="student-name">Baktiar Wasir Farooq</div>
        <span class="student-badge">3rd Year · Kirori Mal College</span>
      </div>
      <ul class="student-works">
        <li>Quantum Information Theoretical Approaches in Neutrino Oscillations <span class="work-type-badge">Dissertation</span></li>
        <li><a href="https://inspirehep.net/literature/3115044" target="_blank">NeutrinoOsc3Flavor: CP Phase Dependence in Three-Flavor Neutrino Oscillations</a></li>
        <li><a href="https://www.sciencedirect.com/science/article/pii/S0550321326000817" target="_blank">Modified Entanglement Patterns in Two-Flavor Neutrinos from Quantum Gravity Interactions</a> — <em>Nuclear Physics B</em></li>
        <li><a href="https://doi.org/10.1142/S021974992540009X" target="_blank">Two-Flavor Neutrino Oscillations in Matter and Quantum Entanglement</a> — <em>Int. Journal of Quantum Information</em></li>
        <li><a href="https://arxiv.org/abs/2604.01256" target="_blank">Quantum Fisher Information as a Probe of Sterile Neutrino New Physics: Geometric Advantage of KM3NeT over IceCube</a></li>
      </ul>
    </div>

    <div class="student-card">
      <div class="student-header">
        <div class="student-name">Ansh Kumariya</div>
        <span class="student-badge">4th Year · Kirori Mal College</span>
      </div>
      <ul class="student-works">
        <li>Day-Night Effects in Solar Neutrino Oscillations: A Comprehensive Review <span class="work-type-badge">Dissertation</span></li>
      </ul>
    </div>

    <div class="student-card">
      <div class="student-header">
        <div class="student-name">Tia Pandit</div>
        <span class="student-badge">4th Year · Kirori Mal College</span>
      </div>
      <ul class="student-works">
        <li>Neutrino Oscillation Experiments: A Comprehensive Review of Theory, Observations and Future Directions <span class="work-type-badge">Dissertation</span></li>
        <li><a href="https://journals.aps.org/prd/accepted/10.1103/8r1c-knd2" target="_blank">Earth-density effects in long baseline neutrino experiments</a> — <em>Physical Review D</em> (Accepted)</li>
      </ul>
    </div>

    <div class="student-card">
      <div class="student-header">
        <div class="student-name">Asta Yadav</div>
        <span class="student-badge">4th Year · Kirori Mal College</span>
      </div>
      <ul class="student-works">
        <li>Introduction to Quantum Cryptography and its Practical Applications <span class="work-type-badge">Dissertation</span></li>
      </ul>
    </div>

    <div class="student-card">
      <div class="student-header">
        <div class="student-name">Hrydia Harish Nambiar</div>
        <span class="student-badge">4th Year · Kirori Mal College</span>
      </div>
      <ul class="student-works">
        <li>Entanglement Aspects of Neutrino Oscillations: A Review <span class="work-type-badge">Dissertation</span></li>
        <li><a href="https://arxiv.org/abs/2605.10972" target="_blank">Tripartite Entanglement as a Probe of Neutrino Mass Hierarchy, CP Violation, and Non-Standard Interactions</a></li>
      </ul>
    </div>

    <div class="student-card">
      <div class="student-header">
        <div class="student-name">Aritro Chatterjee</div>
        <span class="student-badge">3rd Year · Kirori Mal College · Incoming M.Sc. KU Leuven</span>
      </div>
      <ul class="student-works">
        <li><a href="https://arxiv.org/abs/2604.01256" target="_blank">Quantum Fisher Information as a Probe of Sterile Neutrino New Physics: Geometric Advantage of KM3NeT over IceCube</a></li>
      </ul>
    </div>

    <div class="student-card">
      <div class="student-header">
        <div class="student-name">Poulastya Kar</div>
        <span class="student-badge">4th Year · Kirori Mal College</span>
      </div>
      <ul class="student-works">
        <li><a href="https://arxiv.org/abs/2604.00062" target="_blank">Sterile Neutrinos as a Dynamical Cosmological Fluid: Implications for the Expansion History and Matter-Radiation Equality</a></li>
      </ul>
    </div>

    <div class="student-card">
      <div class="student-header">
        <div class="student-name">Mansi Lal</div>
        <span class="student-badge">1st Year Undergrad · Hindu College</span>
      </div>
      <ul class="student-works">
        <li>Extension of CPT Symmetry Models in the case of Neutrino Oscillations</li>
      </ul>
    </div>

    <div class="student-card">
      <div class="student-header">
        <div class="student-name">Abhishek</div>
        <span class="student-badge">1st Year M.Sc. · IIT Bhubaneswar</span>
      </div>
      <ul class="student-works">
        <li>Three-Flavor Neutrino Mixing by Perturbation Approach <span class="work-type-badge">Course Internship</span></li>
      </ul>
    </div>

  </section>

  <footer>
    Prof. Bipin Singh Koranga · Kirori Mal College, University of Delhi · bskoranga@kmc.du.ac.in
  </footer>

</div>
</body>
</html>
