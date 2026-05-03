
<style>
@import url('https://fonts.googleapis.com/css2?family=Syne:wght@400;500;600;700&family=JetBrains+Mono:wght@400;500&display=swap');
*{box-sizing:border-box;margin:0;padding:0}
.gh{font-family:'Syne',sans-serif;color:var(--color-text-primary)}
.sec-label{font-size:11px;font-weight:600;letter-spacing:.13em;text-transform:uppercase;color:#1D9E75;margin-bottom:12px}
.card{background:var(--color-background-primary);border:0.5px solid var(--color-border-tertiary);border-radius:var(--border-radius-lg);padding:1.25rem}
.divider{border:none;border-top:0.5px solid var(--color-border-tertiary);margin:1.5rem 0}

/* HERO */
.hero{display:grid;grid-template-columns:auto 1fr;gap:20px;align-items:start;padding:1.75rem 1.75rem 1.5rem;border-bottom:0.5px solid var(--color-border-tertiary)}
.avatar-wrap{position:relative}
.avatar{width:80px;height:80px;border-radius:50%;background:#085041;display:flex;align-items:center;justify-content:center;font-size:1.5rem;font-weight:700;color:#9FE1CB;letter-spacing:-1px}
.online{position:absolute;bottom:4px;right:4px;width:12px;height:12px;border-radius:50%;background:#1D9E75;border:2px solid var(--color-background-primary)}
.hero-name{font-size:1.55rem;font-weight:700;line-height:1.15;letter-spacing:-.3px}
.hero-username{font-family:'JetBrains Mono',monospace;font-size:.8rem;color:#1D9E75;margin:3px 0 6px}
.hero-bio{font-size:.85rem;color:var(--color-text-secondary);line-height:1.6;max-width:460px}
.hero-meta{display:flex;flex-wrap:wrap;gap:8px 16px;margin-top:10px}
.meta-item{display:flex;align-items:center;gap:5px;font-size:.78rem;color:var(--color-text-secondary)}
.meta-dot{width:6px;height:6px;border-radius:50%;background:#1D9E75;flex-shrink:0}

/* AWARDS */
.awards-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:10px;margin-bottom:1.5rem}
.award-card{background:var(--color-background-secondary);border-radius:var(--border-radius-md);padding:12px;border-left:3px solid}
.award-card.nasa{border-color:#378ADD}
.award-card.icpc{border-color:#EF9F27}
.award-card.global{border-color:#1D9E75}
.award-title{font-size:.8rem;font-weight:600;margin-bottom:3px}
.award-sub{font-size:.72rem;color:var(--color-text-secondary);line-height:1.4}

/* BADGES ROW */
.badge-row{display:flex;flex-wrap:wrap;gap:7px;margin-bottom:1.5rem}
.badge{font-size:.7rem;font-weight:500;padding:4px 10px;border-radius:20px;border:0.5px solid;letter-spacing:.04em}
.b-teal{background:#E1F5EE;color:#085041;border-color:#5DCAA5}
.b-blue{background:#E6F1FB;color:#0C447C;border-color:#85B7EB}
.b-amber{background:#FAEEDA;color:#633806;border-color:#FAC775}
.b-gray{background:#F1EFE8;color:#444441;border-color:#B4B2A9}

/* SKILLS */
.skills-wrap{display:grid;grid-template-columns:1fr 1fr;gap:1.5rem;margin-bottom:1.5rem}
.skill-group-name{font-size:.68rem;font-weight:600;letter-spacing:.1em;text-transform:uppercase;color:var(--color-text-tertiary);margin-bottom:7px}
.tags{display:flex;flex-wrap:wrap;gap:5px}
.tag{font-family:'JetBrains Mono',monospace;font-size:.72rem;padding:3px 8px;border-radius:5px;background:var(--color-background-secondary);color:var(--color-text-secondary);border:0.5px solid var(--color-border-tertiary)}
.tag-hi{background:#E1F5EE;color:#085041;border-color:#5DCAA5}

/* CURRENTLY */
.currently-bar{display:flex;align-items:center;gap:10px;padding:10px 14px;background:var(--color-background-secondary);border-radius:var(--border-radius-md);margin-bottom:1.5rem;font-size:.82rem}
.pulse{width:8px;height:8px;border-radius:50%;background:#1D9E75;flex-shrink:0;animation:pulse 2s infinite}
@keyframes pulse{0%,100%{opacity:1}50%{opacity:.3}}

/* PROFILES */
.profiles-grid{display:grid;grid-template-columns:repeat(2,1fr);gap:8px;margin-bottom:1.5rem}
.profile-item{display:flex;align-items:center;gap:9px;padding:9px 12px;border:0.5px solid var(--color-border-tertiary);border-radius:var(--border-radius-md);font-size:.8rem;color:var(--color-text-secondary);cursor:pointer;text-decoration:none}
.profile-item:hover{background:var(--color-background-secondary)}
.p-dot{width:8px;height:8px;border-radius:50%;flex-shrink:0}
.pd-gh{background:#444441}
.pd-li{background:#185FA5}
.pd-tw{background:#378ADD}
.pd-so{background:#EF9F27}
.pd-kg{background:#1D9E75}
.pd-fb{background:#185FA5}
.pd-ig{background:#D4537E}
.pd-yt{background:#E24B4A}
.pd-cf{background:#D85A30}
.pd-cc{background:#EF9F27}
.pd-hr{background:#1D9E75}
.pd-lc{background:#BA7517}
.pd-he{background:#1D9E75}
.pd-dc{background:#7F77DD}
.pd-dev{background:#444441}
.pd-ss{background:#378ADD}

/* BLOGS */
.blog-section{margin-bottom:1.5rem}
.blog-note{font-size:.8rem;color:var(--color-text-secondary);font-style:italic;padding:10px 14px;background:var(--color-background-secondary);border-radius:var(--border-radius-md)}

/* STATS */
.stats-row{display:grid;grid-template-columns:repeat(4,1fr);gap:10px;margin-bottom:1.5rem}
.stat{background:var(--color-background-secondary);border-radius:var(--border-radius-md);padding:12px;text-align:center}
.stat-n{font-size:1.3rem;font-weight:700;color:#1D9E75;font-family:'JetBrains Mono',monospace}
.stat-l{font-size:.68rem;color:var(--color-text-secondary);margin-top:3px;letter-spacing:.03em}

/* FOOTER */
.footer{display:flex;align-items:center;justify-content:space-between;flex-wrap:wrap;gap:10px;padding:1.25rem 1.75rem 1.5rem;border-top:0.5px solid var(--color-border-tertiary)}
.footer-mono{font-family:'JetBrains Mono',monospace;font-size:.68rem;color:var(--color-text-tertiary)}
.footer-email{font-size:.78rem;color:#1D9E75;text-decoration:none}
.footer-views{font-size:.72rem;color:var(--color-text-tertiary);display:flex;align-items:center;gap:5px}

/* SECTION WRAPPER */
.body{padding:1.5rem 1.75rem 0}
</style>

<h2 class="sr-only">GitHub profile of Md. Asraful Molla — Python & Django developer, competitive programmer, NASA Space Apps champion</h2>

<div class="gh">

  <div class="hero">
    <div class="avatar-wrap">
      <div class="avatar">AM</div>
      <div class="online"></div>
    </div>
    <div>
      <div class="hero-name">Md. Asraful Molla</div>
      <div class="hero-username">@asrafulmolla</div>
      <div class="hero-bio">Python &amp; Django Developer · C, C++, JavaScript · AI/ML Enthusiast · Competitive Programmer</div>
      <div class="hero-meta">
        <span class="meta-item"><span class="meta-dot"></span>Dhaka International University — CSE</span>
        <span class="meta-item"><span class="meta-dot"></span><a href="https://asraful.theuniqueonlineshop.com" style="color:inherit;text-decoration:none">asraful.theuniqueonlineshop.com</a></span>
        <span class="meta-item"><span class="meta-dot"></span>asraful@students.diu.ac</span>
      </div>
    </div>
  </div>

  <div class="body">

    <div class="currently-bar">
      <span class="pulse"></span>
      <span>Currently learning — <strong>Advanced Django &amp; AI/ML</strong></span>
    </div>

    <div class="sec-label">Achievements &amp; honors</div>
    <div class="awards-grid">
      <div class="award-card nasa">
        <div class="award-title">NASA Space Apps 2025</div>
        <div class="award-sub">Champion (Barisal) · Global Nominee · Honorable Mention</div>
      </div>
      <div class="award-card icpc">
        <div class="award-title">ICPC Asia Dhaka 2024</div>
        <div class="award-sub">Honorable Mention — International Collegiate Programming Contest</div>
      </div>
      <div class="award-card global">
        <div class="award-title">B.Sc. CSE — ongoing</div>
        <div class="award-sub">Dhaka International University · Problem-solving &amp; research focus</div>
      </div>
    </div>

    <div class="sec-label">Profile views &amp; stats</div>
    <div class="stats-row">
      <div class="stat"><div class="stat-n">6+</div><div class="stat-l">Coding platforms</div></div>
      <div class="stat"><div class="stat-n">3+</div><div class="stat-l">International awards</div></div>
      <div class="stat"><div class="stat-n">15+</div><div class="stat-l">Technologies</div></div>
      <div class="stat"><div class="stat-n">14+</div><div class="stat-l">Social &amp; dev links</div></div>
    </div>

    <div class="sec-label">Languages &amp; tools</div>
    <div class="skills-wrap">
      <div>
        <div class="skill-group-name">Languages</div>
        <div class="tags" style="margin-bottom:12px">
          <span class="tag tag-hi">Python</span><span class="tag tag-hi">C++</span><span class="tag">C</span><span class="tag">JavaScript</span><span class="tag">Java</span>
        </div>
        <div class="skill-group-name">Frameworks &amp; UI</div>
        <div class="tags" style="margin-bottom:12px">
          <span class="tag tag-hi">Django</span><span class="tag">React</span><span class="tag">React Native</span><span class="tag">Bootstrap</span><span class="tag">Tailwind CSS</span><span class="tag">D3.js</span>
        </div>
        <div class="skill-group-name">Data &amp; ML</div>
        <div class="tags">
          <span class="tag">Pandas</span><span class="tag">AI/ML</span>
        </div>
      </div>
      <div>
        <div class="skill-group-name">Databases</div>
        <div class="tags" style="margin-bottom:12px">
          <span class="tag">PostgreSQL</span><span class="tag">MySQL</span><span class="tag">MongoDB</span><span class="tag">SQLite</span><span class="tag">MSSQL</span>
        </div>
        <div class="skill-group-name">Cloud &amp; DevOps</div>
        <div class="tags" style="margin-bottom:12px">
          <span class="tag">Docker</span><span class="tag">AWS</span><span class="tag">GCP</span><span class="tag">Git</span><span class="tag">Linux</span>
        </div>
        <div class="skill-group-name">Design &amp; Hardware</div>
        <div class="tags">
          <span class="tag">Figma</span><span class="tag">Arduino</span>
        </div>
      </div>
    </div>

    <div class="sec-label">Projects &amp; writing</div>
    <div class="badge-row">
      <span class="badge b-teal">Projects → asraful.theuniqueonlineshop.com</span>
      <span class="badge b-blue">Blog → /blog/</span>
      <span class="badge b-gray">Resume → PDF available</span>
    </div>

    <div class="blog-section">
      <div class="blog-note">Blog posts are updated regularly at <a href="https://asraful.theuniqueonlineshop.com/blog/" style="color:#1D9E75">asraful.theuniqueonlineshop.com/blog/</a> — topics span Django, AI/ML, and competitive programming.</div>
    </div>

    <div class="sec-label">Connect &amp; coding profiles</div>
    <div class="profiles-grid">
      <a class="profile-item" href="https://dev.to/mdasrafulmolla"><span class="p-dot pd-dev"></span>Dev.to — mdasrafulmolla</a>
      <a class="profile-item" href="https://twitter.com/arasrafulmolla"><span class="p-dot pd-tw"></span>Twitter / X — @arasrafulmolla</a>
      <a class="profile-item" href="https://linkedin.com/in/mdasrafulmolla"><span class="p-dot pd-li"></span>LinkedIn — mdasrafulmolla</a>
      <a class="profile-item" href="https://stackoverflow.com/users/28672220"><span class="p-dot pd-so"></span>Stack Overflow — 28672220</a>
      <a class="profile-item" href="https://kaggle.com/mdasrafulmolla"><span class="p-dot pd-kg"></span>Kaggle — mdasrafulmolla</a>
      <a class="profile-item" href="https://fb.com/mdasrafulmolla4"><span class="p-dot pd-fb"></span>Facebook — mdasrafulmolla4</a>
      <a class="profile-item" href="https://instagram.com/mdasrafulmolla4"><span class="p-dot pd-ig"></span>Instagram — mdasrafulmolla4</a>
      <a class="profile-item" href="https://www.youtube.com/c/@mdasrafulmolla1"><span class="p-dot pd-yt"></span>YouTube — @mdasrafulmolla1</a>
      <a class="profile-item" href="https://www.codechef.com/users/mdasraful"><span class="p-dot pd-cc"></span>CodeChef — mdasraful</a>
      <a class="profile-item" href="https://www.hackerrank.com/armdasraful"><span class="p-dot pd-hr"></span>HackerRank — armdasraful</a>
      <a class="profile-item" href="https://codeforces.com/profile/asraful.diu"><span class="p-dot pd-cf"></span>Codeforces — asraful.diu</a>
      <a class="profile-item" href="https://www.leetcode.com/mdasrafulmolla"><span class="p-dot pd-lc"></span>LeetCode — mdasrafulmolla</a>
      <a class="profile-item" href="https://www.hackerearth.com/@armdasraful"><span class="p-dot pd-he"></span>HackerEarth — @armdasraful</a>
      <a class="profile-item" href="https://discord.gg/mdasrafulmolla"><span class="p-dot pd-dc"></span>Discord — mdasrafulmolla</a>
      <a class="profile-item" href="https://www.stopstalk.com/user/profile/mdasrafulmolla"><span class="p-dot pd-ss"></span>StopStalk — mdasrafulmolla</a>
      <a class="profile-item" href="https://asraful.theuniqueonlineshop.com/media/resumes/MD_x9XfPWR._ASRAFUL_MOLLA.pdf"><span class="p-dot pd-kg"></span>Resume — download PDF</a>
    </div>

  </div>

  <div class="footer">
    <div class="footer-mono">01001101 01100100 00101110 00100000 01000001 01110011 01110010 01100001 01100110 01110101 01101100</div>
    <a class="footer-email" href="mailto:asraful@students.diu.ac">asraful@students.diu.ac</a>
  </div>

</div>
