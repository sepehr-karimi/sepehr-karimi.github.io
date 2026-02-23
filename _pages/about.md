---
permalink: /
title: ""
author_profile: false
redirect_from:
  - /about/
  - /about.html
---

<style>
/* ── Reset Jekyll/Minimal Mistakes interference ── */
.masthead { display: none !important; }
.page__footer { display: none !important; }
#main { padding: 0 !important; max-width: 100% !important; float: none !important; width: 100% !important; }
.page { padding: 0 !important; max-width: 100% !important; float: none !important; width: 100% !important; }
.page__inner-wrap { padding: 0 !important; float: none !important; width: 100% !important; margin: 0 !important; }
.page__content { padding: 0 !important; width: 100% !important; float: none !important; }
.initial-content { padding: 0 !important; }
.sidebar { display: none !important; }
.sidebar__right { display: none !important; }
article.page { margin: 0 !important; padding: 0 !important; }
body { background: #f4f8fc !important; }
/* Force full bleed */
.page__hero, .page__hero--overlay { display: none !important; }
#page-title { display: none !important; }
h1.page__title { display: none !important; }

/* ── Variables ── */
:root {
  --blue: #0077b6;
  --blue-dark: #023e8a;
  --blue-deep: #03045e;
  --blue-light: #90e0ef;
  --blue-pale: #caf0f8;
  --text: #0d1b2a;
  --muted: #5a6a7a;
  --border: #e2eaf2;
  --card: #fff;
  --bg: #f4f8fc;
  --radius: 12px;
}

* { margin: 0; padding: 0; box-sizing: border-box; }
body { font-family: 'Inter', 'Segoe UI', sans-serif; color: var(--text); line-height: 1.6; }

/* ── Custom Nav ── */
.sk-nav { background: #fff; border-bottom: 1px solid var(--border); position: sticky; top: 0; z-index: 100; box-shadow: 0 1px 8px rgba(0,0,0,.06); }
.sk-nav-inner { max-width: 1100px; margin: auto; padding: 0 2rem; display: flex; align-items: center; justify-content: space-between; height: 60px; }
.sk-nav-logo { font-weight: 700; font-size: 1.1rem; color: var(--blue-dark); text-decoration: none; }
.sk-nav-links { display: flex; gap: 1.8rem; list-style: none; }
.sk-nav-links a { text-decoration: none; color: var(--muted); font-size: .9rem; font-weight: 500; transition: color .2s; }
.sk-nav-links a:hover { color: var(--blue); }

/* ── Hero ── */
.sk-hero { background: linear-gradient(135deg, var(--blue-deep) 0%, var(--blue-dark) 50%, var(--blue) 100%); padding: 5rem 2rem 4rem; position: relative; overflow: hidden; }
.sk-hero::before { content: ''; position: absolute; inset: 0; opacity: .03; background-image: radial-gradient(circle, #fff 1px, transparent 1px); background-size: 30px 30px; }
.sk-hero-inner { max-width: 1100px; margin: auto; display: flex; align-items: center; gap: 3rem; position: relative; }
.sk-hero-photo { flex-shrink: 0; }
.sk-hero-photo img { width: 160px; height: 160px; border-radius: 50%; border: 4px solid rgba(255,255,255,.3); object-fit: cover; box-shadow: 0 8px 32px rgba(0,0,0,.3); }
.sk-hero-placeholder { width: 160px; height: 160px; border-radius: 50%; border: 4px solid rgba(255,255,255,.3); background: linear-gradient(135deg, #48cae4, #0077b6); display: flex; align-items: center; justify-content: center; font-size: 3rem; color: white; box-shadow: 0 8px 32px rgba(0,0,0,.3); font-weight: 700; }
.sk-hero-content { color: white; }
.sk-hero-content h1 { font-size: 2.6rem; font-weight: 800; margin-bottom: .4rem; line-height: 1.2; color: white; border: none; }
.sk-hero-role { font-size: 1.1rem; color: var(--blue-light); font-weight: 500; margin-bottom: .3rem; }
.sk-hero-affil { font-size: .95rem; color: rgba(255,255,255,.7); margin-bottom: 1.4rem; }
.sk-tags { display: flex; flex-wrap: wrap; gap: .5rem; margin-bottom: 1.6rem; }
.sk-tag { background: rgba(255,255,255,.12); border: 1px solid rgba(255,255,255,.2); color: white; padding: 4px 12px; border-radius: 20px; font-size: .8rem; font-weight: 500; }
.sk-btns { display: flex; flex-wrap: wrap; gap: .7rem; }
.sk-btn { padding: .55rem 1.3rem; border-radius: 8px; font-size: .88rem; font-weight: 600; text-decoration: none; display: inline-flex; align-items: center; gap: .4rem; transition: all .2s; }
.sk-btn-white { background: white; color: var(--blue-dark) !important; }
.sk-btn-white:hover { background: var(--blue-pale); transform: translateY(-1px); }
.sk-btn-outline { background: transparent; color: white !important; border: 2px solid rgba(255,255,255,.5); }
.sk-btn-outline:hover { border-color: white; background: rgba(255,255,255,.1); transform: translateY(-1px); }

/* ── Social strip ── */
.sk-social { background: var(--blue-dark); padding: .7rem 2rem; }
.sk-social-inner { max-width: 1100px; margin: auto; display: flex; gap: 1.5rem; align-items: center; flex-wrap: wrap; }
.sk-social a { color: rgba(255,255,255,.7); text-decoration: none; font-size: .85rem; transition: color .2s; }
.sk-social a:hover { color: white; }

/* ── Main layout ── */
.sk-main { max-width: 1100px; margin: 2.5rem auto; padding: 0 2rem; display: grid; grid-template-columns: 1fr 320px; gap: 2rem; }

/* ── Cards ── */
.sk-card { background: var(--card); border-radius: var(--radius); padding: 1.6rem; border: 1px solid var(--border); box-shadow: 0 2px 12px rgba(0,0,0,.05); margin-bottom: 1.5rem; }
.sk-card h2 { font-size: 1.1rem; font-weight: 700; color: var(--blue-dark); margin-bottom: 1rem; display: flex; align-items: center; gap: .5rem; border: none; padding: 0; }
.sk-card h2::after { content: ''; flex: 1; height: 2px; background: linear-gradient(90deg, var(--blue-pale), transparent); margin-left: .5rem; }

/* ── About ── */
.sk-about p { color: var(--muted); font-size: .93rem; margin-bottom: .8rem; line-height: 1.7; }
.sk-interests { display: flex; flex-wrap: wrap; gap: .5rem; margin-top: .8rem; }
.sk-interest { background: var(--blue-pale); color: var(--blue-dark); padding: 4px 12px; border-radius: 20px; font-size: .8rem; font-weight: 500; }

/* ── Publications ── */
.sk-pub { border: 1px solid var(--border); border-left: 4px solid var(--blue); border-radius: 8px; padding: 1rem 1.2rem; margin-bottom: 1rem; transition: all .2s; background: #fff; }
.sk-pub:hover { transform: translateY(-2px); box-shadow: 0 6px 20px rgba(0,119,182,.1); }
.sk-badges { display: flex; gap: .4rem; margin-bottom: .5rem; }
.sk-badge { font-size: .68rem; font-weight: 700; padding: 2px 8px; border-radius: 20px; text-transform: uppercase; letter-spacing: .05em; }
.sk-badge-year { background: #e0f2fe; color: #0369a1; }
.sk-badge-conf { background: #fef3c7; color: #92400e; }
.sk-badge-pre { background: #f3e8ff; color: #6d28d9; }
.sk-pub-title { font-size: .93rem; font-weight: 600; color: var(--text); margin-bottom: .3rem; line-height: 1.4; }
.sk-pub-authors { font-size: .82rem; color: var(--muted); margin-bottom: .2rem; }
.sk-pub-venue { font-size: .82rem; color: #8a9bb0; font-style: italic; margin-bottom: .6rem; }
.sk-pub-links { display: flex; gap: .5rem; }
.sk-lnk { padding: 3px 10px; border-radius: 6px; font-size: .75rem; font-weight: 600; text-decoration: none; transition: all .2s; display: inline-block; color: white !important; }
.sk-lnk-arxiv { background: #b91c1c; }
.sk-lnk-arxiv:hover { background: #991b1b; }
.sk-lnk-springer { background: #0077b6; }
.sk-lnk-springer:hover { background: #023e8a; }

/* ── News ── */
.sk-news-item { display: flex; gap: 1rem; padding: .8rem 0; border-bottom: 1px solid var(--border); }
.sk-news-item:last-child { border-bottom: none; }
.sk-news-date { font-size: .75rem; color: var(--muted); white-space: nowrap; padding-top: .15rem; min-width: 80px; }
.sk-news-body a { font-size: .88rem; font-weight: 600; color: var(--text); text-decoration: none; }
.sk-news-body a:hover { color: var(--blue); }
.sk-news-body p { font-size: .82rem; color: var(--muted); margin-top: .2rem; }

/* ── Sidebar ── */
.sk-stat-grid { display: grid; grid-template-columns: 1fr 1fr; gap: .8rem; margin-bottom: .3rem; }
.sk-stat { background: var(--bg); border-radius: 8px; padding: .8rem; text-align: center; border: 1px solid var(--border); }
.sk-stat-num { font-size: 1.5rem; font-weight: 800; color: var(--blue); }
.sk-stat-label { font-size: .72rem; color: var(--muted); font-weight: 500; }

.sk-edu-item { display: flex; gap: .8rem; padding: .7rem 0; border-bottom: 1px solid var(--border); }
.sk-edu-item:last-child { border-bottom: none; }
.sk-edu-dot { width: 10px; height: 10px; border-radius: 50%; margin-top: .35rem; flex-shrink: 0; }
.sk-edu-deg { font-size: .85rem; font-weight: 600; color: var(--text); }
.sk-edu-uni { font-size: .78rem; color: var(--muted); }
.sk-edu-year { font-size: .74rem; color: var(--blue); font-weight: 600; }

.sk-skill-group { margin-bottom: .9rem; }
.sk-skill-label { font-size: .8rem; font-weight: 600; color: var(--muted); margin-bottom: .4rem; text-transform: uppercase; letter-spacing: .06em; display: block; }
.sk-skills { display: flex; flex-wrap: wrap; gap: .4rem; }
.sk-skill { background: var(--bg); border: 1px solid var(--border); color: var(--text); padding: 3px 10px; border-radius: 6px; font-size: .78rem; font-weight: 500; }

.sk-exp-item { padding: .7rem 0; border-bottom: 1px solid var(--border); }
.sk-exp-item:last-child { border-bottom: none; }
.sk-exp-role { font-size: .87rem; font-weight: 600; color: var(--text); }
.sk-exp-company { font-size: .8rem; color: var(--blue); font-weight: 500; }
.sk-exp-period { font-size: .75rem; color: var(--muted); }

.sk-contact-btn { display: block; text-align: center; padding: .65rem; border-radius: 8px; font-weight: 600; font-size: .88rem; text-decoration: none; transition: all .2s; margin-bottom: .6rem; }
.sk-contact-primary { background: var(--blue); color: white !important; }
.sk-contact-primary:hover { background: var(--blue-dark); }
.sk-contact-secondary { background: var(--bg); color: var(--text) !important; border: 1px solid var(--border); }
.sk-contact-secondary:hover { border-color: var(--blue); color: var(--blue) !important; }

/* ── Footer ── */
.sk-footer { background: var(--blue-deep); color: rgba(255,255,255,.6); text-align: center; padding: 1.5rem; font-size: .82rem; margin-top: 2rem; }
.sk-footer a { color: var(--blue-light); text-decoration: none; }

/* ── Responsive ── */
@media (max-width: 768px) {
  .sk-main { grid-template-columns: 1fr; }
  .sk-hero-inner { flex-direction: column; text-align: center; }
  .sk-tags, .sk-btns { justify-content: center; }
  .sk-hero-content h1 { font-size: 2rem; }
  .sk-nav-links { display: none; }
}
</style>

<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet"/>

<!-- NAV -->
<nav class="sk-nav">
  <div class="sk-nav-inner">
    <a href="/" class="sk-nav-logo">Sepehr Karimi</a>
    <ul class="sk-nav-links">
      <li><a href="#about">About</a></li>
      <li><a href="#publications">Publications</a></li>
      <li><a href="#news">News</a></li>
      <li><a href="/teaching/">Teaching</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </div>
</nav>

<!-- HERO -->
<section class="sk-hero">
  <div class="sk-hero-inner">
    <div class="sk-hero-photo">
      <img src="/images/profile-site.jpg" alt="Sepehr Karimi"/>
    </div>
    <div class="sk-hero-content">
      <h1>Sepehr Karimi</h1>
      <p class="sk-hero-role">PhD Researcher in AI &amp; Energy Systems</p>
      <p class="sk-hero-affil">📍 University of Adelaide · Supervised by Dr. Ali Pourmousavi Kani</p>
      <div class="sk-tags">
        <span class="sk-tag">Machine Learning</span>
        <span class="sk-tag">Energy Forecasting</span>
        <span class="sk-tag">Reinforcement Learning</span>
        <span class="sk-tag">NLP</span>
        <span class="sk-tag">BESS Optimization</span>
      </div>
      <div class="sk-btns">
        <a href="/files/cv.pdf" class="sk-btn sk-btn-white">📄 Download CV</a>
        <a href="https://scholar.google.com/citations?user=k4954-QAAAAJ" class="sk-btn sk-btn-outline" target="_blank">🎓 Google Scholar</a>
        <a href="mailto:sepkarimia@gmail.com" class="sk-btn sk-btn-outline">✉️ Email Me</a>
        <a href="https://github.com/sepehr-karimi" class="sk-btn sk-btn-outline" target="_blank">💻 GitHub</a>
      </div>
    </div>
  </div>
</section>

<!-- SOCIAL STRIP -->
<div class="sk-social">
  <div class="sk-social-inner">
    <a href="mailto:sepkarimia@gmail.com">✉️ sepkarimia@gmail.com</a>
    <a href="https://www.linkedin.com/in/sepehrkarimia" target="_blank">🔗 LinkedIn</a>
    <a href="https://github.com/sepehr-karimi" target="_blank">💻 GitHub</a>
    <a href="https://scholar.google.com/citations?user=k4954-QAAAAJ" target="_blank">🎓 Google Scholar</a>
  </div>
</div>

<!-- MAIN -->
<div class="sk-main">

  <!-- LEFT -->
  <div>

    <div class="sk-card" id="about">
      <h2>👤 About Me</h2>
      <div class="sk-about">
        <p>I am a <strong>Machine Learning and AI researcher</strong> pursuing my <strong>PhD at the University of Adelaide</strong>, Australia, under the supervision of <strong>Dr. Ali Pourmousavi Kani</strong>. My research focuses on developing <strong>unified, data-driven frameworks</strong> for electricity price forecasting and battery energy storage system (BESS) operation in the Australian National Electricity Market (NEM).</p>
        <p>Before starting my PhD, I completed my <strong>Master's degree in Computer Engineering</strong> at the University of Tehran, where I worked at the NLP Lab on domain-specific QA, LLM-based conversational agents, and multilingual chatbot systems. I have also collaborated with research groups at <strong>Columbia University</strong> and <strong>Nottingham Trent University</strong> on clinical NLP, EEG-based disease detection, and multimodal deep learning.</p>
        <div class="sk-interests">
          <span class="sk-interest">⚡ Electricity Price Forecasting</span>
          <span class="sk-interest">🔋 Energy Storage Optimization</span>
          <span class="sk-interest">📈 Time-Series Modeling</span>
          <span class="sk-interest">🧠 NLP &amp; LLMs</span>
          <span class="sk-interest">🤖 Reinforcement Learning</span>
        </div>
      </div>
    </div>

    <div class="sk-card" id="publications">
      <h2>📚 Selected Publications</h2>

      <div class="sk-pub">
        <div class="sk-badges">
          <span class="sk-badge sk-badge-year">2025</span>
          <span class="sk-badge sk-badge-pre">Preprint</span>
        </div>
        <div class="sk-pub-title">Speech-Based Cognitive Screening: A Systematic Evaluation of LLM Adaptation Strategies</div>
        <div class="sk-pub-authors"><strong>Sepehr Karimi</strong>, Fatemeh Taherinezhad, M.J. Momeni Nezhad, Sina Rashidi, et al.</div>
        <div class="sk-pub-venue">arXiv:2509.03525, 2025</div>
        <div class="sk-pub-links">
          <a href="https://arxiv.org/abs/2509.03525" class="sk-lnk sk-lnk-arxiv" target="_blank">arXiv</a>
        </div>
      </div>

      <div class="sk-pub">
        <div class="sk-badges">
          <span class="sk-badge sk-badge-year">2025</span>
          <span class="sk-badge sk-badge-pre">Preprint</span>
        </div>
        <div class="sk-pub-title">PersianMedQA: Language-Centric Evaluation of LLMs in the Persian Medical Domain</div>
        <div class="sk-pub-authors">M.J. Ranjbar Kalahroodi, <strong>Sepehr Karimi*</strong>, A. Sheikholselami*, et al.</div>
        <div class="sk-pub-venue">arXiv:2506.00250, 2025</div>
        <div class="sk-pub-links">
          <a href="https://arxiv.org/abs/2506.00250" class="sk-lnk sk-lnk-arxiv" target="_blank">arXiv</a>
        </div>
      </div>

      <div class="sk-pub">
        <div class="sk-badges">
          <span class="sk-badge sk-badge-year">2024</span>
          <span class="sk-badge sk-badge-conf">Conference</span>
        </div>
        <div class="sk-pub-title">Deep Learning Approaches in EEG Analysis for Early Detection of Alzheimer's Disease and MCI</div>
        <div class="sk-pub-authors">T. Morovati*, H. Vaezi*, <strong>Sepehr Karimi*</strong>, Md Mahmud, et al.</div>
        <div class="sk-pub-venue">Int. Conference on Applied Intelligence and Informatics, pp. 63–81, 2024</div>
        <div class="sk-pub-links">
          <a href="https://link.springer.com/chapter/10.1007/978-3-032-04657-4_5" class="sk-lnk sk-lnk-springer" target="_blank">Springer</a>
        </div>
      </div>

      <p style="font-size:.85rem;color:var(--muted);margin-top:.5rem">
        Full list on <a href="https://scholar.google.com/citations?user=k4954-QAAAAJ" target="_blank" style="color:var(--blue)">Google Scholar →</a>
      </p>
    </div>

    <div class="sk-card" id="news">
      <h2>📰 Recent News</h2>
      <div class="sk-news-item">
        <div class="sk-news-date">Nov 2025</div>
        <div class="sk-news-body">
          <a href="/blog/2024/09/starting-phd-adelaide/">Starting PhD at the University of Adelaide</a>
          <p>Commenced PhD supported by a National Industry PhD Project with OptiGrid Pty Ltd. ⚡</p>
        </div>
      </div>
      <div class="sk-news-item">
        <div class="sk-news-date">Mar 2024</div>
        <div class="sk-news-body">
          <a href="/blog/2024/03/sofia-mind-university-tehran/">SofiaMind's First Client — University of Tehran</a>
          <p>Successfully deployed a chatbot system for university services and student inquiries.</p>
        </div>
      </div>
      <div class="sk-news-item">
        <div class="sk-news-date">Mar 2024</div>
        <div class="sk-news-body">
          <a href="/blog/2024/03/research-assistantship-nottingham-trent/">Research Assistantship @ Nottingham Trent University</a>
          <p>Systematic review of deep learning on EEG for Alzheimer's detection.</p>
        </div>
      </div>
      <div class="sk-news-item">
        <div class="sk-news-date">Jan 2024</div>
        <div class="sk-news-body">
          <a href="/blog/2024/01/research-assistantship-columbia/">Research Assistantship @ Columbia University</a>
          <p>Joined Dr. Maryam Zolnoori's group, working on LLMs for clinical decision support.</p>
        </div>
      </div>
    </div>

  </div>

  <!-- SIDEBAR -->
  <div>

    <div class="sk-card">
      <h2>📊 At a Glance</h2>
      <div class="sk-stat-grid">
        <div class="sk-stat"><div class="sk-stat-num">3</div><div class="sk-stat-label">Publications</div></div>
        <div class="sk-stat"><div class="sk-stat-num">2+</div><div class="sk-stat-label">Years Research</div></div>
        <div class="sk-stat"><div class="sk-stat-num">3</div><div class="sk-stat-label">Institutions</div></div>
        <div class="sk-stat"><div class="sk-stat-num">2</div><div class="sk-stat-label">Companies</div></div>
      </div>
    </div>

    <div class="sk-card">
      <h2>🎓 Education</h2>
      <div class="sk-edu-item">
        <div class="sk-edu-dot" style="background:#0077b6"></div>
        <div>
          <div class="sk-edu-deg">PhD, Electrical &amp; Electronic Eng.</div>
          <div class="sk-edu-uni">University of Adelaide</div>
          <div class="sk-edu-year">2025 – Present</div>
        </div>
      </div>
      <div class="sk-edu-item">
        <div class="sk-edu-dot" style="background:#48cae4"></div>
        <div>
          <div class="sk-edu-deg">M.Sc., Computer Engineering</div>
          <div class="sk-edu-uni">University of Tehran</div>
          <div class="sk-edu-year">2021 – 2024</div>
        </div>
      </div>
      <div class="sk-edu-item">
        <div class="sk-edu-dot" style="background:#90e0ef"></div>
        <div>
          <div class="sk-edu-deg">B.Sc., Electrical Engineering</div>
          <div class="sk-edu-uni">Amirkabir University of Technology</div>
          <div class="sk-edu-year">2016 – 2021</div>
        </div>
      </div>
    </div>

    <div class="sk-card">
      <h2>🛠️ Skills</h2>
      <div class="sk-skill-group">
        <span class="sk-skill-label">ML / AI</span>
        <div class="sk-skills">
          <span class="sk-skill">PyTorch</span><span class="sk-skill">TensorFlow</span>
          <span class="sk-skill">Transformers</span><span class="sk-skill">RL</span><span class="sk-skill">LLMs</span>
        </div>
      </div>
      <div class="sk-skill-group">
        <span class="sk-skill-label">Data &amp; Engineering</span>
        <div class="sk-skills">
          <span class="sk-skill">Python</span><span class="sk-skill">Pandas</span>
          <span class="sk-skill">SQL</span><span class="sk-skill">FastAPI</span><span class="sk-skill">Docker</span>
        </div>
      </div>
      <div class="sk-skill-group">
        <span class="sk-skill-label">Energy Systems</span>
        <div class="sk-skills">
          <span class="sk-skill">BESS Optimization</span><span class="sk-skill">NEM Analytics</span>
          <span class="sk-skill">Price Forecasting</span>
        </div>
      </div>
    </div>

    <div class="sk-card">
      <h2>💼 Experience</h2>
      <div class="sk-exp-item">
        <div class="sk-exp-role">Data Scientist &amp; Backend Engineer</div>
        <div class="sk-exp-company">OptiGrid Pty Ltd</div>
        <div class="sk-exp-period">Oct 2023 – Present</div>
      </div>
      <div class="sk-exp-item">
        <div class="sk-exp-role">Co-Founder &amp; AI Engineer</div>
        <div class="sk-exp-company">SofiaMind</div>
        <div class="sk-exp-period">Sep 2023 – Present</div>
      </div>
      <div class="sk-exp-item">
        <div class="sk-exp-role">Research Assistant</div>
        <div class="sk-exp-company">Columbia University</div>
        <div class="sk-exp-period">Jan 2024 – Present</div>
      </div>
      <div class="sk-exp-item">
        <div class="sk-exp-role">Research Assistant</div>
        <div class="sk-exp-company">Nottingham Trent University</div>
        <div class="sk-exp-period">Mar 2024 – Present</div>
      </div>
    </div>

    <div class="sk-card" id="contact">
      <h2>📬 Contact</h2>
      <a href="/files/cv.pdf" class="sk-contact-btn sk-contact-primary">📄 Download CV</a>
      <a href="mailto:sepkarimia@gmail.com" class="sk-contact-btn sk-contact-secondary">✉️ sepkarimia@gmail.com</a>
      <a href="https://www.linkedin.com/in/sepehrkarimia" class="sk-contact-btn sk-contact-secondary" target="_blank">🔗 LinkedIn</a>
      <a href="https://github.com/sepehr-karimi" class="sk-contact-btn sk-contact-secondary" target="_blank">💻 GitHub</a>
    </div>

  </div>
</div>

<div class="sk-footer">
  © 2025 Sepehr Karimi · University of Adelaide ·
  <a href="mailto:sepkarimia@gmail.com">sepkarimia@gmail.com</a>
</div>
