---
permalink: /
title: ""
author_profile: false
redirect_from:
  - /about/
  - /about.html
---

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Sepehr Karimi</title>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet"/>
<style>
*{margin:0;padding:0;box-sizing:border-box}
:root{
  --blue:#0077b6;--blue-dark:#023e8a;--blue-deep:#03045e;
  --blue-light:#90e0ef;--blue-pale:#caf0f8;
  --text:#0d1b2a;--muted:#5a6a7a;--border:#e2eaf2;
  --card:#fff;--bg:#f4f8fc;
}
body{font-family:'Inter',sans-serif;background:var(--bg);color:var(--text);line-height:1.6}

/* NAV */
nav{background:#fff;border-bottom:1px solid var(--border);position:sticky;top:0;z-index:100;box-shadow:0 1px 8px rgba(0,0,0,.06)}
.nav-inner{max-width:1100px;margin:auto;padding:0 2rem;display:flex;align-items:center;justify-content:space-between;height:60px}
.nav-logo{font-weight:700;font-size:1.1rem;color:var(--blue-dark);text-decoration:none}
.nav-links{display:flex;gap:1.8rem;list-style:none}
.nav-links a{text-decoration:none;color:var(--muted);font-size:.9rem;font-weight:500;transition:color .2s}
.nav-links a:hover{color:var(--blue)}

/* HERO */
.hero{background:linear-gradient(135deg,var(--blue-deep) 0%,var(--blue-dark) 50%,var(--blue) 100%);padding:5rem 2rem 4rem;position:relative;overflow:hidden}
.hero::before{content:'';position:absolute;inset:0;background:url("data:image/svg+xml,%3Csvg width='60' height='60' viewBox='0 0 60 60' xmlns='http://www.w3.org/2000/svg'%3E%3Cg fill='none' fill-rule='evenodd'%3E%3Cg fill='%23ffffff' fill-opacity='0.03'%3E%3Cpath d='M36 34v-4h-2v4h-4v2h4v4h2v-4h4v-2h-4zm0-30V0h-2v4h-4v2h4v4h2V6h4V4h-4zM6 34v-4H4v4H0v2h4v4h2v-4h4v-2H6zM6 4V0H4v4H0v2h4v4h2V6h4V4H6z'/%3E%3C/g%3E%3C/g%3E%3C/svg%3E")}
.hero-inner{max-width:1100px;margin:auto;display:flex;align-items:center;gap:3rem;position:relative}
.hero-photo{flex-shrink:0}
.hero-photo img{width:160px;height:160px;border-radius:50%;border:4px solid rgba(255,255,255,.3);object-fit:cover;box-shadow:0 8px 32px rgba(0,0,0,.3)}
.hero-photo-placeholder{width:160px;height:160px;border-radius:50%;border:4px solid rgba(255,255,255,.3);background:linear-gradient(135deg,#48cae4,#0077b6);display:flex;align-items:center;justify-content:center;font-size:3rem;color:white;box-shadow:0 8px 32px rgba(0,0,0,.3)}
.hero-content{color:white}
.hero-content h1{font-size:2.6rem;font-weight:800;margin-bottom:.4rem;line-height:1.2}
.hero-role{font-size:1.1rem;color:var(--blue-light);font-weight:500;margin-bottom:.3rem}
.hero-affil{font-size:.95rem;color:rgba(255,255,255,.7);margin-bottom:1.4rem}
.hero-tags{display:flex;flex-wrap:wrap;gap:.5rem;margin-bottom:1.6rem}
.tag{background:rgba(255,255,255,.12);border:1px solid rgba(255,255,255,.2);color:white;padding:4px 12px;border-radius:20px;font-size:.8rem;font-weight:500}
.hero-btns{display:flex;flex-wrap:wrap;gap:.7rem}
.btn{padding:.55rem 1.3rem;border-radius:8px;font-size:.88rem;font-weight:600;text-decoration:none;display:inline-flex;align-items:center;gap:.4rem;transition:all .2s;cursor:pointer;border:none}
.btn-white{background:white;color:var(--blue-dark)}
.btn-white:hover{background:var(--blue-pale);transform:translateY(-1px)}
.btn-outline{background:transparent;color:white;border:2px solid rgba(255,255,255,.5)}
.btn-outline:hover{border-color:white;background:rgba(255,255,255,.1);transform:translateY(-1px)}

/* SOCIAL STRIP */
.social-strip{background:var(--blue-dark);padding:.7rem 2rem}
.social-inner{max-width:1100px;margin:auto;display:flex;gap:1.5rem;align-items:center;flex-wrap:wrap}
.social-link{color:rgba(255,255,255,.7);text-decoration:none;font-size:.85rem;display:flex;align-items:center;gap:.4rem;transition:color .2s}
.social-link:hover{color:white}
.social-link svg{width:16px;height:16px;fill:currentColor}

/* MAIN LAYOUT */
.main{max-width:1100px;margin:2.5rem auto;padding:0 2rem;display:grid;grid-template-columns:1fr 320px;gap:2rem}

/* CARDS */
.card{background:var(--card);border-radius:12px;padding:1.6rem;border:1px solid var(--border);box-shadow:0 2px 12px rgba(0,0,0,.05);margin-bottom:1.5rem}
.card h2{font-size:1.1rem;font-weight:700;color:var(--blue-dark);margin-bottom:1rem;display:flex;align-items:center;gap:.5rem}
.card h2::after{content:'';flex:1;height:2px;background:linear-gradient(90deg,var(--blue-pale),transparent);margin-left:.5rem}

/* ABOUT */
.about-text p{color:var(--muted);font-size:.93rem;margin-bottom:.8rem;line-height:1.7}
.interests{display:flex;flex-wrap:wrap;gap:.5rem;margin-top:.8rem}
.interest-tag{background:var(--blue-pale);color:var(--blue-dark);padding:4px 12px;border-radius:20px;font-size:.8rem;font-weight:500}

/* PUBLICATIONS */
.pub-card{border:1px solid var(--border);border-left:4px solid var(--blue);border-radius:8px;padding:1rem 1.2rem;margin-bottom:1rem;transition:all .2s;background:#fff}
.pub-card:hover{transform:translateY(-2px);box-shadow:0 6px 20px rgba(0,119,182,.1);border-left-color:var(--blue-dark)}
.pub-badges{display:flex;gap:.4rem;margin-bottom:.5rem}
.badge{font-size:.68rem;font-weight:700;padding:2px 8px;border-radius:20px;text-transform:uppercase;letter-spacing:.05em}
.badge-year{background:#e0f2fe;color:#0369a1}
.badge-conf{background:#fef3c7;color:#92400e}
.badge-preprint{background:#f3e8ff;color:#6d28d9}
.pub-title{font-size:.93rem;font-weight:600;color:var(--text);margin-bottom:.3rem;line-height:1.4}
.pub-authors{font-size:.82rem;color:var(--muted);margin-bottom:.2rem}
.pub-venue{font-size:.82rem;color:#8a9bb0;font-style:italic;margin-bottom:.6rem}
.pub-links{display:flex;gap:.5rem}
.btn-xs{padding:3px 10px;border-radius:6px;font-size:.75rem;font-weight:600;text-decoration:none;transition:all .2s;display:inline-block}
.btn-arxiv{background:#b91c1c;color:white}
.btn-arxiv:hover{background:#991b1b}
.btn-springer{background:#0077b6;color:white}
.btn-springer:hover{background:#023e8a}

/* NEWS */
.news-item{display:flex;gap:1rem;padding:.8rem 0;border-bottom:1px solid var(--border)}
.news-item:last-child{border-bottom:none}
.news-date{font-size:.75rem;color:var(--muted);white-space:nowrap;padding-top:.15rem;min-width:80px}
.news-body a{font-size:.88rem;font-weight:600;color:var(--text);text-decoration:none}
.news-body a:hover{color:var(--blue)}
.news-body p{font-size:.82rem;color:var(--muted);margin-top:.2rem}

/* SIDEBAR */
.sidebar{}
.stat-grid{display:grid;grid-template-columns:1fr 1fr;gap:.8rem;margin-bottom:.3rem}
.stat-box{background:var(--bg);border-radius:8px;padding:.8rem;text-align:center;border:1px solid var(--border)}
.stat-num{font-size:1.5rem;font-weight:800;color:var(--blue)}
.stat-label{font-size:.72rem;color:var(--muted);font-weight:500}

.edu-item{display:flex;gap:.8rem;padding:.7rem 0;border-bottom:1px solid var(--border)}
.edu-item:last-child{border-bottom:none}
.edu-dot{width:10px;height:10px;border-radius:50%;background:var(--blue);margin-top:.35rem;flex-shrink:0}
.edu-deg{font-size:.85rem;font-weight:600;color:var(--text)}
.edu-uni{font-size:.78rem;color:var(--muted)}
.edu-year{font-size:.74rem;color:var(--blue);font-weight:600}

.skill-group{margin-bottom:.9rem}
.skill-label{font-size:.8rem;font-weight:600;color:var(--muted);margin-bottom:.4rem;text-transform:uppercase;letter-spacing:.06em}
.skills{display:flex;flex-wrap:wrap;gap:.4rem}
.skill{background:var(--bg);border:1px solid var(--border);color:var(--text);padding:3px 10px;border-radius:6px;font-size:.78rem;font-weight:500}

.exp-item{padding:.7rem 0;border-bottom:1px solid var(--border)}
.exp-item:last-child{border-bottom:none}
.exp-role{font-size:.87rem;font-weight:600;color:var(--text)}
.exp-company{font-size:.8rem;color:var(--blue);font-weight:500}
.exp-period{font-size:.75rem;color:var(--muted)}

.contact-btn{display:block;text-align:center;padding:.65rem;border-radius:8px;font-weight:600;font-size:.88rem;text-decoration:none;transition:all .2s;margin-bottom:.6rem}
.contact-primary{background:var(--blue);color:white}
.contact-primary:hover{background:var(--blue-dark)}
.contact-secondary{background:var(--bg);color:var(--text);border:1px solid var(--border)}
.contact-secondary:hover{border-color:var(--blue);color:var(--blue)}

/* FOOTER */
footer{background:var(--blue-deep);color:rgba(255,255,255,.6);text-align:center;padding:1.5rem;font-size:.82rem;margin-top:2rem}
footer a{color:var(--blue-light);text-decoration:none}

@media(max-width:768px){
  .main{grid-template-columns:1fr}
  .hero-inner{flex-direction:column;text-align:center}
  .hero-tags,.hero-btns{justify-content:center}
  .hero-content h1{font-size:2rem}
}
</style>
</head>
<body>

<!-- NAV -->
<nav>
  <div class="nav-inner">
    <a href="#" class="nav-logo">Sepehr Karimi</a>
    <ul class="nav-links">
      <li><a href="#about">About</a></li>
      <li><a href="#publications">Publications</a></li>
      <li><a href="#news">News</a></li>
      <li><a href="#teaching">Teaching</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </div>
</nav>

<!-- HERO -->
<section class="hero">
  <div class="hero-inner">
    <div class="hero-photo">
      <div class="hero-photo-placeholder">SK</div>
      <!-- Replace above with: <img src="/images/profile-site.jpg" alt="Sepehr Karimi"/> -->
    </div>
    <div class="hero-content">
      <h1>Sepehr Karimi</h1>
      <p class="hero-role">PhD Researcher in AI &amp; Energy Systems</p>
      <p class="hero-affil">📍 University of Adelaide · Supervised by Dr. Ali Pourmousavi Kani</p>
      <div class="hero-tags">
        <span class="tag">Machine Learning</span>
        <span class="tag">Energy Forecasting</span>
        <span class="tag">Reinforcement Learning</span>
        <span class="tag">NLP</span>
        <span class="tag">BESS Optimization</span>
      </div>
      <div class="hero-btns">
        <a href="/files/cv.pdf" class="btn btn-white">📄 Download CV</a>
        <a href="https://scholar.google.com/citations?user=k4954-QAAAAJ" class="btn btn-outline" target="_blank">🎓 Google Scholar</a>
        <a href="mailto:sepkarimia@gmail.com" class="btn btn-outline">✉️ Email Me</a>
        <a href="https://github.com/sepehr-karimi" class="btn btn-outline" target="_blank">💻 GitHub</a>
      </div>
    </div>
  </div>
</section>

<!-- SOCIAL STRIP -->
<div class="social-strip">
  <div class="social-inner">
    <a href="mailto:sepkarimia@gmail.com" class="social-link">✉️ sepkarimia@gmail.com</a>
    <a href="https://www.linkedin.com/in/sepehrkarimia" class="social-link" target="_blank">🔗 LinkedIn</a>
    <a href="https://github.com/sepehr-karimi" class="social-link" target="_blank">💻 GitHub</a>
    <a href="https://scholar.google.com/citations?user=k4954-QAAAAJ" class="social-link" target="_blank">🎓 Google Scholar</a>
  </div>
</div>

<!-- MAIN -->
<div class="main">
  <!-- LEFT COLUMN -->
  <div>

    <!-- ABOUT -->
    <div class="card" id="about">
      <h2>👤 About Me</h2>
      <div class="about-text">
        <p>I am a <strong>Machine Learning and AI researcher</strong> pursuing my <strong>PhD at the University of Adelaide</strong>, Australia, under the supervision of <strong>Dr. Ali Pourmousavi Kani</strong>. My research focuses on developing <strong>unified, data-driven frameworks</strong> for electricity price forecasting and battery energy storage system (BESS) operation in the Australian National Electricity Market (NEM).</p>
        <p>Before starting my PhD, I completed my <strong>Master's degree in Computer Engineering</strong> at the University of Tehran, where I worked at the NLP Lab on domain-specific QA, LLM-based conversational agents, and multilingual chatbot systems. I have also collaborated with research groups at <strong>Columbia University</strong> and <strong>Nottingham Trent University</strong> on clinical NLP, EEG-based disease detection, and multimodal deep learning.</p>
        <div class="interests">
          <span class="interest-tag">⚡ Electricity Price Forecasting</span>
          <span class="interest-tag">🔋 Energy Storage Optimization</span>
          <span class="interest-tag">📈 Time-Series Modeling</span>
          <span class="interest-tag">🧠 NLP & LLMs</span>
          <span class="interest-tag">🤖 Reinforcement Learning</span>
        </div>
      </div>
    </div>

    <!-- PUBLICATIONS -->
    <div class="card" id="publications">
      <h2>📚 Selected Publications</h2>

      <div class="pub-card">
        <div class="pub-badges">
          <span class="badge badge-year">2025</span>
          <span class="badge badge-preprint">Preprint</span>
        </div>
        <div class="pub-title">Speech-Based Cognitive Screening: A Systematic Evaluation of LLM Adaptation Strategies</div>
        <div class="pub-authors"><strong>Sepehr Karimi</strong>, Fatemeh Taherinezhad, M.J. Momeni Nezhad, Sina Rashidi, et al.</div>
        <div class="pub-venue">arXiv:2509.03525, 2025</div>
        <div class="pub-links">
          <a href="https://arxiv.org/abs/2509.03525" class="btn-xs btn-arxiv" target="_blank">arXiv</a>
        </div>
      </div>

      <div class="pub-card">
        <div class="pub-badges">
          <span class="badge badge-year">2025</span>
          <span class="badge badge-preprint">Preprint</span>
        </div>
        <div class="pub-title">PersianMedQA: Language-Centric Evaluation of LLMs in the Persian Medical Domain</div>
        <div class="pub-authors">M.J. Ranjbar Kalahroodi, <strong>Sepehr Karimi*</strong>, A. Sheikholselami*, et al.</div>
        <div class="pub-venue">arXiv:2506.00250, 2025</div>
        <div class="pub-links">
          <a href="https://arxiv.org/abs/2506.00250" class="btn-xs btn-arxiv" target="_blank">arXiv</a>
        </div>
      </div>

      <div class="pub-card">
        <div class="pub-badges">
          <span class="badge badge-year">2024</span>
          <span class="badge badge-conf">Conference</span>
        </div>
        <div class="pub-title">Deep Learning Approaches in EEG Analysis for Early Detection of Alzheimer's Disease and MCI: A Mini Systematic Review</div>
        <div class="pub-authors">T. Morovati*, H. Vaezi*, <strong>Sepehr Karimi*</strong>, Md Mahmud, M. Crook-Rumsey, et al.</div>
        <div class="pub-venue">Int. Conference on Applied Intelligence and Informatics, pp. 63–81, 2024</div>
        <div class="pub-links">
          <a href="https://link.springer.com/chapter/10.1007/978-3-032-04657-4_5" class="btn-xs btn-springer" target="_blank">Springer</a>
        </div>
      </div>

      <p style="font-size:.85rem;color:var(--muted);margin-top:.5rem">
        See full list on <a href="https://scholar.google.com/citations?user=k4954-QAAAAJ" target="_blank" style="color:var(--blue)">Google Scholar →</a>
      </p>
    </div>

    <!-- NEWS -->
    <div class="card" id="news">
      <h2>📰 Recent News</h2>
      <div class="news-item">
        <div class="news-date">Nov 2025</div>
        <div class="news-body">
          <a href="#">Starting PhD at the University of Adelaide</a>
          <p>Officially commenced PhD supported by a National Industry PhD Project with OptiGrid Pty Ltd. ⚡</p>
        </div>
      </div>
      <div class="news-item">
        <div class="news-date">Mar 2024</div>
        <div class="news-body">
          <a href="#">SofiaMind's First Client — University of Tehran</a>
          <p>Successfully deployed a chatbot system for university services and student inquiries.</p>
        </div>
      </div>
      <div class="news-item">
        <div class="news-date">Mar 2024</div>
        <div class="news-body">
          <a href="#">Research Assistantship @ Nottingham Trent University</a>
          <p>Joined remotely to conduct a systematic review of deep learning on EEG for Alzheimer's detection.</p>
        </div>
      </div>
      <div class="news-item">
        <div class="news-date">Jan 2024</div>
        <div class="news-body">
          <a href="#">Research Assistantship @ Columbia University</a>
          <p>Joined Dr. Maryam Zolnoori's group, working on LLMs for clinical decision support.</p>
        </div>
      </div>
    </div>

  </div>

  <!-- RIGHT SIDEBAR -->
  <div class="sidebar">

    <!-- STATS -->
    <div class="card">
      <h2>📊 At a Glance</h2>
      <div class="stat-grid">
        <div class="stat-box"><div class="stat-num">3</div><div class="stat-label">Publications</div></div>
        <div class="stat-box"><div class="stat-num">2+</div><div class="stat-label">Years Research</div></div>
        <div class="stat-box"><div class="stat-num">3</div><div class="stat-label">Institutions</div></div>
        <div class="stat-box"><div class="stat-num">2</div><div class="stat-label">Companies</div></div>
      </div>
    </div>

    <!-- EDUCATION -->
    <div class="card">
      <h2>🎓 Education</h2>
      <div class="edu-item">
        <div class="edu-dot" style="background:#0077b6"></div>
        <div>
          <div class="edu-deg">PhD, Electrical &amp; Electronic Eng.</div>
          <div class="edu-uni">University of Adelaide</div>
          <div class="edu-year">2025 – Present</div>
        </div>
      </div>
      <div class="edu-item">
        <div class="edu-dot" style="background:#48cae4"></div>
        <div>
          <div class="edu-deg">M.Sc., Computer Engineering</div>
          <div class="edu-uni">University of Tehran</div>
          <div class="edu-year">2021 – 2024</div>
        </div>
      </div>
      <div class="edu-item">
        <div class="edu-dot" style="background:#90e0ef"></div>
        <div>
          <div class="edu-deg">B.Sc., Electrical Engineering</div>
          <div class="edu-uni">Amirkabir University of Technology</div>
          <div class="edu-year">2016 – 2021</div>
        </div>
      </div>
    </div>

    <!-- SKILLS -->
    <div class="card">
      <h2>🛠️ Skills</h2>
      <div class="skill-group">
        <div class="skill-label">ML / AI</div>
        <div class="skills">
          <span class="skill">PyTorch</span><span class="skill">TensorFlow</span>
          <span class="skill">Transformers</span><span class="skill">RL</span><span class="skill">LLMs</span>
        </div>
      </div>
      <div class="skill-group">
        <div class="skill-label">Data & Engineering</div>
        <div class="skills">
          <span class="skill">Python</span><span class="skill">Pandas</span>
          <span class="skill">SQL</span><span class="skill">FastAPI</span><span class="skill">Docker</span>
        </div>
      </div>
      <div class="skill-group">
        <div class="skill-label">Energy Systems</div>
        <div class="skills">
          <span class="skill">BESS Optimization</span><span class="skill">NEM Analytics</span>
          <span class="skill">Price Forecasting</span>
        </div>
      </div>
    </div>

    <!-- EXPERIENCE -->
    <div class="card">
      <h2>💼 Experience</h2>
      <div class="exp-item">
        <div class="exp-role">Data Scientist &amp; Backend Engineer</div>
        <div class="exp-company">OptiGrid Pty Ltd</div>
        <div class="exp-period">Oct 2023 – Present</div>
      </div>
      <div class="exp-item">
        <div class="exp-role">Co-Founder &amp; AI Engineer</div>
        <div class="exp-company">SofiaMind</div>
        <div class="exp-period">Sep 2023 – Present</div>
      </div>
      <div class="exp-item">
        <div class="exp-role">Research Assistant</div>
        <div class="exp-company">Columbia University</div>
        <div class="exp-period">Jan 2024 – Present</div>
      </div>
      <div class="exp-item">
        <div class="exp-role">Research Assistant</div>
        <div class="exp-company">Nottingham Trent University</div>
        <div class="exp-period">Mar 2024 – Present</div>
      </div>
    </div>

    <!-- CONTACT -->
    <div class="card" id="contact">
      <h2>📬 Contact</h2>
      <a href="/files/cv.pdf" class="contact-btn contact-primary">📄 Download CV</a>
      <a href="mailto:sepkarimia@gmail.com" class="contact-btn contact-secondary">✉️ sepkarimia@gmail.com</a>
      <a href="https://www.linkedin.com/in/sepehrkarimia" class="contact-btn contact-secondary" target="_blank">🔗 LinkedIn</a>
      <a href="https://github.com/sepehr-karimi" class="contact-btn contact-secondary" target="_blank">💻 GitHub</a>
    </div>

  </div>
</div>

<footer>
  © 2025 Sepehr Karimi · University of Adelaide ·
  <a href="mailto:sepkarimia@gmail.com">sepkarimia@gmail.com</a>
</footer>

</body>
</html>
