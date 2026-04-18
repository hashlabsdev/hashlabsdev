<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Hash Labs</title>
<link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@400;500;600;700&family=JetBrains+Mono:wght@400;500&display=swap" rel="stylesheet"/>
<style>
  *, *::before, *::after { margin: 0; padding: 0; box-sizing: border-box; }

  body {
    font-family: 'Space Grotesk', sans-serif;
    background: #0a0a0f;
    color: #e2e0f0;
    min-height: 100vh;
  }

  a { text-decoration: none; color: inherit; }

  /* ── BANNER ── */
  .banner {
    position: relative;
    padding: 60px 40px 50px;
    text-align: center;
    background: #0c0c16;
    overflow: hidden;
    border-bottom: 1px solid #1a1a2e;
  }

  .banner-grid {
    position: absolute;
    inset: 0;
    background-image:
      linear-gradient(rgba(99,80,230,0.06) 1px, transparent 1px),
      linear-gradient(90deg, rgba(99,80,230,0.06) 1px, transparent 1px);
    background-size: 44px 44px;
  }

  .banner-glow {
    position: absolute;
    top: -80px; left: 50%;
    transform: translateX(-50%);
    width: 560px; height: 340px;
    background: radial-gradient(ellipse, rgba(99,80,230,0.15) 0%, transparent 65%);
    pointer-events: none;
  }

  .logo-row {
    position: relative;
    z-index: 2;
    display: inline-flex;
    align-items: center;
    gap: 14px;
    margin-bottom: 10px;
  }

  .logo-mark {
    width: 48px; height: 48px;
    background: linear-gradient(135deg, #6350e6 0%, #a07aff 100%);
    border-radius: 12px;
    display: flex; align-items: center; justify-content: center;
    font-family: 'JetBrains Mono', monospace;
    font-size: 22px; font-weight: 500;
    color: #fff;
    box-shadow: 0 0 28px rgba(99,80,230,0.45);
  }

  .banner h1 {
    font-size: 48px;
    font-weight: 700;
    letter-spacing: -1.5px;
    color: #fff;
  }

  .banner-tagline {
    position: relative;
    z-index: 2;
    font-size: 11px;
    letter-spacing: 4px;
    text-transform: uppercase;
    color: #4a4a6a;
    font-weight: 500;
    margin-bottom: 20px;
  }

  .banner-badges {
    position: relative;
    z-index: 2;
    display: inline-flex;
    gap: 10px;
  }

  .bbadge {
    display: inline-flex;
    align-items: center;
    gap: 6px;
    padding: 5px 14px;
    border-radius: 20px;
    font-size: 12px;
    font-weight: 500;
    border: 1px solid;
    cursor: pointer;
    transition: opacity 0.15s;
  }
  .bbadge:hover { opacity: 0.8; }

  .bbadge-ig {
    background: rgba(228,64,95,0.12);
    border-color: rgba(228,64,95,0.35);
    color: #e4405f;
  }

  .bbadge-li {
    background: rgba(79,156,249,0.1);
    border-color: rgba(79,156,249,0.3);
    color: #4f9cf9;
  }

  .bdot {
    width: 6px; height: 6px;
    border-radius: 50%;
    background: currentColor;
    animation: bpulse 2s infinite;
  }

  @keyframes bpulse { 0%,100%{opacity:1} 50%{opacity:0.35} }

  /* ── WRAPPER ── */
  .page { max-width: 860px; margin: 0 auto; padding: 0 40px 80px; }

  /* ── SEPARATOR ── */
  .sep {
    height: 1px;
    background: linear-gradient(90deg, transparent, #1e1e32 20%, #252538 50%, #1e1e32 80%, transparent);
    margin: 44px 0;
  }

  /* ── SECTION LABEL ── */
  .sec-label {
    display: flex;
    align-items: center;
    gap: 10px;
    margin-bottom: 14px;
  }

  .sec-icon {
    width: 28px; height: 28px;
    border-radius: 7px;
    background: rgba(99,80,230,0.14);
    border: 1px solid rgba(99,80,230,0.28);
    display: flex; align-items: center; justify-content: center;
    font-size: 13px;
  }

  .sec-title {
    font-family: 'JetBrains Mono', monospace;
    font-size: 11px;
    font-weight: 600;
    letter-spacing: 3px;
    text-transform: uppercase;
    color: #6350e6;
  }

  /* ── HEADINGS ── */
  h2 {
    font-size: 28px;
    font-weight: 700;
    color: #fff;
    letter-spacing: -0.5px;
    margin-bottom: 14px;
  }

  p {
    font-size: 14px;
    line-height: 1.8;
    color: #7a7a9e;
  }

  em { font-style: normal; color: #a07aff; font-weight: 500; }

  /* ── QUOTE ── */
  .quote {
    border-left: 2px solid #252542;
    padding: 10px 18px;
    margin-top: 18px;
  }

  .quote p {
    font-size: 13px;
    font-style: italic;
    color: #4a4a6a;
  }

  /* ── BUILD CARDS ── */
  .build-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 14px;
    margin-top: 22px;
  }

  .build-card {
    background: #111120;
    border: 1px solid #1e1e32;
    border-radius: 12px;
    padding: 22px 18px;
    transition: border-color 0.2s, transform 0.2s;
  }

  .build-card:hover {
    border-color: rgba(99,80,230,0.35);
    transform: translateY(-3px);
  }

  .build-icon { font-size: 24px; margin-bottom: 12px; display: block; }

  .build-title {
    font-size: 13px;
    font-weight: 600;
    color: #c8c8e8;
    margin-bottom: 8px;
  }

  .build-desc {
    font-size: 12px;
    color: #4a4a6a;
    line-height: 1.65;
  }

  /* ── STACK ── */
  .stack-section { margin-top: 22px; }

  .stack-group { margin-bottom: 20px; }

  .stack-group-label {
    font-family: 'JetBrains Mono', monospace;
    font-size: 10px;
    font-weight: 600;
    letter-spacing: 2.5px;
    text-transform: uppercase;
    color: #3a3a54;
    margin-bottom: 10px;
  }

  .tags { display: flex; flex-wrap: wrap; gap: 7px; }

  .tag {
    display: inline-flex;
    align-items: center;
    gap: 5px;
    padding: 5px 13px;
    border-radius: 6px;
    font-size: 12px;
    font-weight: 500;
    font-family: 'JetBrains Mono', monospace;
    border: 1px solid;
    transition: transform 0.15s;
    cursor: default;
  }

  .tag:hover { transform: scale(1.04); }

  .tag-red    { background:rgba(255,45,32,.08); border-color:rgba(255,45,32,.25); color:#ff6b5b; }
  .tag-purple { background:rgba(119,107,180,.1);border-color:rgba(119,107,180,.28);color:#a09ac8;}
  .tag-green  { background:rgba(52,211,100,.08);border-color:rgba(52,211,100,.25);color:#4ade80; }
  .tag-black  { background:rgba(255,255,255,.05);border-color:rgba(255,255,255,.14);color:#c8c8e0;}
  .tag-blue   { background:rgba(63,131,248,.09);border-color:rgba(63,131,248,.25);color:#5ba3ff; }
  .tag-ts     { background:rgba(49,120,198,.1); border-color:rgba(49,120,198,.28); color:#60a5fa; }
  .tag-cyan   { background:rgba(6,182,212,.08); border-color:rgba(6,182,212,.25); color:#22d3ee; }
  .tag-pgblue { background:rgba(65,105,225,.1); border-color:rgba(65,105,225,.28); color:#7ba4ff; }
  .tag-mysql  { background:rgba(68,121,161,.1); border-color:rgba(68,121,161,.28); color:#5ba3c8; }
  .tag-redis  { background:rgba(220,56,45,.1);  border-color:rgba(220,56,45,.28); color:#f87171; }
  .tag-sky    { background:rgba(56,189,248,.08);border-color:rgba(56,189,248,.25);color:#38bdf8; }
  .tag-rn     { background:rgba(32,35,42,.5);   border-color:rgba(97,218,251,.2); color:#61dafb; }
  .tag-flutter{ background:rgba(2,86,155,.1);   border-color:rgba(2,86,155,.3);   color:#38bdf8; }

  /* ── FOCUS BOX ── */
  .focus-box {
    background: #0f0f1c;
    border: 1px solid rgba(99,80,230,0.22);
    border-left: 3px solid #6350e6;
    border-radius: 12px;
    padding: 26px 28px;
    margin-top: 22px;
    position: relative;
    overflow: hidden;
  }

  .focus-box::before {
    content: '';
    position: absolute;
    top: -50px; right: -50px;
    width: 200px; height: 200px;
    background: radial-gradient(ellipse, rgba(99,80,230,0.07), transparent 70%);
    pointer-events: none;
  }

  .focus-title {
    font-size: 15px;
    font-weight: 700;
    color: #fff;
    margin-bottom: 4px;
  }

  .focus-sub {
    font-family: 'JetBrains Mono', monospace;
    font-size: 11px;
    color: #3a3a5a;
    margin-bottom: 20px;
  }

  .feat-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 10px 24px;
  }

  .feat-item {
    display: flex;
    align-items: flex-start;
    gap: 8px;
    font-size: 12.5px;
    color: #6a6a8a;
    line-height: 1.5;
  }

  .feat-dot {
    width: 5px; height: 5px;
    border-radius: 50%;
    background: #6350e6;
    margin-top: 5px;
    flex-shrink: 0;
  }

  /* ── MINDSET ── */
  .mindset-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 12px;
    margin-top: 22px;
  }

  .mindset-card {
    background: #0f0f1a;
    border: 1px solid #1a1a2c;
    border-radius: 10px;
    padding: 18px;
  }

  .mindset-title {
    font-family: 'JetBrains Mono', monospace;
    font-size: 12px;
    font-weight: 500;
    color: #a07aff;
    margin-bottom: 7px;
  }

  .mindset-body {
    font-size: 12px;
    color: #4a4a68;
    line-height: 1.65;
  }

  /* ── FOLLOW ── */
  .follow-row {
    display: flex;
    gap: 12px;
    margin-top: 22px;
  }

  .social-btn {
    display: inline-flex;
    align-items: center;
    gap: 9px;
    padding: 11px 20px;
    border-radius: 8px;
    font-size: 13px;
    font-weight: 600;
    cursor: pointer;
    transition: transform 0.15s, opacity 0.15s;
    text-decoration: none;
  }

  .social-btn:hover { transform: translateY(-2px); opacity: 0.9; }

  .btn-ig {
    background: rgba(228,64,95,0.12);
    border: 1px solid rgba(228,64,95,0.3);
    color: #e4405f;
  }

  .btn-li {
    background: rgba(79,156,249,0.1);
    border: 1px solid rgba(79,156,249,0.28);
    color: #4f9cf9;
  }

  /* ── FOOTER ── */
  .footer {
    text-align: center;
    padding-top: 44px;
    margin-top: 44px;
    border-top: 1px solid #16162a;
  }

  .footer-text {
    font-family: 'JetBrains Mono', monospace;
    font-size: 11px;
    color: #28283e;
    letter-spacing: 1.5px;
  }
</style>
</head>
<body>

<!-- BANNER -->
<div class="banner">
  <div class="banner-grid"></div>
  <div class="banner-glow"></div>
  <div class="logo-row">
    <div class="logo-mark">#</div>
    <h1>Hash Labs</h1>
  </div>
  <div class="banner-tagline">Engineering Digital Products That Matter</div>
  <div class="banner-badges">
    <a href="https://www.instagram.com/hashc_oding" class="bbadge bbadge-ig" target="_blank">
      <span class="bdot"></span> @hashc_oding
    </a>
    <a href="https://www.linkedin.com/in/hash-company" class="bbadge bbadge-li" target="_blank">
      <span class="bdot"></span> Hash_Company
    </a>
  </div>
</div>

<!-- PAGE CONTENT -->
<div class="page">

  <!-- WHO WE ARE -->
  <div class="sep"></div>
  <div class="sec-label">
    <div class="sec-icon">🏢</div>
    <div class="sec-title">About</div>
  </div>
  <h2>Who We Are</h2>
  <p>
    <em>Hash Labs</em> is a software company that builds digital products for businesses demanding reliability
    and precision. We specialize in custom web applications, POS systems, and mobile apps —
    engineered from the ground up with performance-first architecture and clean, maintainable code.
  </p>
  <div class="quote">
    <p>"We don't just write code — we engineer systems."</p>
  </div>

  <!-- WHAT WE BUILD -->
  <div class="sep"></div>
  <div class="sec-label">
    <div class="sec-icon">🔨</div>
    <div class="sec-title">Products</div>
  </div>
  <h2>What We Build</h2>
  <div class="build-grid">
    <div class="build-card">
      <span class="build-icon">🌐</span>
      <div class="build-title">Web Applications</div>
      <div class="build-desc">Scalable, modern platforms built for speed and usability — from dashboards to full SaaS products.</div>
    </div>
    <div class="build-card">
      <span class="build-icon">🖥️</span>
      <div class="build-title">POS Systems</div>
      <div class="build-desc">Purpose-built point-of-sale for Pharmacy and Retail — inventory, billing, and reporting in one system.</div>
    </div>
    <div class="build-card">
      <span class="build-icon">📱</span>
      <div class="build-title">Mobile Apps</div>
      <div class="build-desc">Cross-platform mobile applications that are fast, intuitive, and ready for production.</div>
    </div>
  </div>

  <!-- TECH STACK -->
  <div class="sep"></div>
  <div class="sec-label">
    <div class="sec-icon">⚙️</div>
    <div class="sec-title">Stack</div>
  </div>
  <h2>Tech Stack</h2>
  <div class="stack-section">
    <div class="stack-group">
      <div class="stack-group-label">Backend</div>
      <div class="tags">
        <span class="tag tag-red">◉ Laravel</span>
        <span class="tag tag-purple">◈ PHP</span>
        <span class="tag tag-green">⬡ Node.js</span>
      </div>
    </div>
    <div class="stack-group">
      <div class="stack-group-label">Frontend</div>
      <div class="tags">
        <span class="tag tag-black">▲ Next.js</span>
        <span class="tag tag-rn">◉ React</span>
        <span class="tag tag-ts">{} TypeScript</span>
        <span class="tag tag-cyan">∿ Tailwind CSS</span>
      </div>
    </div>
    <div class="stack-group">
      <div class="stack-group-label">Database &amp; Infrastructure</div>
      <div class="tags">
        <span class="tag tag-pgblue">◍ PostgreSQL</span>
        <span class="tag tag-mysql">◍ MySQL</span>
        <span class="tag tag-redis">◉ Redis</span>
        <span class="tag tag-sky">⬡ Docker</span>
      </div>
    </div>
    <div class="stack-group">
      <div class="stack-group-label">Mobile</div>
      <div class="tags">
        <span class="tag tag-rn">◉ React Native</span>
        <span class="tag tag-flutter">◈ Flutter</span>
      </div>
    </div>
  </div>

  <!-- CURRENT FOCUS -->
  <div class="sep"></div>
  <div class="sec-label">
    <div class="sec-icon">🎯</div>
    <div class="sec-title">Focus</div>
  </div>
  <h2>Current Focus</h2>
  <div class="focus-box">
    <div class="focus-title">💊 Pharmacy POS System</div>
    <div class="focus-sub">Laravel · Next.js · PostgreSQL — Production-grade, not a prototype.</div>
    <div class="feat-grid">
      <div class="feat-item"><span class="feat-dot"></span>Inventory &amp; stock expiry tracking</div>
      <div class="feat-item"><span class="feat-dot"></span>Billing, invoicing &amp; receipt printing</div>
      <div class="feat-item"><span class="feat-dot"></span>Supplier &amp; purchase order management</div>
      <div class="feat-item"><span class="feat-dot"></span>Sales analytics &amp; reporting dashboard</div>
      <div class="feat-item"><span class="feat-dot"></span>Customer profiles &amp; purchase history</div>
      <div class="feat-item"><span class="feat-dot"></span>Role-based access control</div>
    </div>
  </div>

  <!-- HOW WE THINK -->
  <div class="sep"></div>
  <div class="sec-label">
    <div class="sec-icon">🧠</div>
    <div class="sec-title">Mindset</div>
  </div>
  <h2>How We Think</h2>
  <div class="mindset-grid">
    <div class="mindset-card">
      <div class="mindset-title">// clean_code</div>
      <div class="mindset-body">No shortcuts. Readable, maintainable architecture is non-negotiable.</div>
    </div>
    <div class="mindset-card">
      <div class="mindset-title">// systems_thinking</div>
      <div class="mindset-body">We design for scale from day one — not as an afterthought.</div>
    </div>
    <div class="mindset-card">
      <div class="mindset-title">// ship_it</div>
      <div class="mindset-body">Ideas are nothing without execution. We build and we deliver.</div>
    </div>
    <div class="mindset-card">
      <div class="mindset-title">// always_improving</div>
      <div class="mindset-body">Every sprint is a chance to do it better than the last.</div>
    </div>
  </div>

  <!-- FOLLOW US -->
  <div class="sep"></div>
  <div class="sec-label">
    <div class="sec-icon">🤝</div>
    <div class="sec-title">Connect</div>
  </div>
  <h2>Follow Us</h2>
  <p>Stay updated with what we're shipping.</p>
  <div class="follow-row">
    <a class="social-btn btn-ig" href="https://www.instagram.com/hashc_oding" target="_blank">
      <svg width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
        <rect x="2" y="2" width="20" height="20" rx="5" ry="5"/>
        <path d="M16 11.37A4 4 0 1 1 12.63 8 4 4 0 0 1 16 11.37z"/>
        <line x1="17.5" y1="6.5" x2="17.51" y2="6.5"/>
      </svg>
      @hashc_oding
    </a>
    <a class="social-btn btn-li" href="https://www.linkedin.com/in/hash-company" target="_blank">
      <svg width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
        <path d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"/>
        <rect x="2" y="9" width="4" height="12"/>
        <circle cx="4" cy="4" r="2"/>
      </svg>
      Hash Company
    </a>
  </div>

  <!-- FOOTER -->
  <div class="footer">
    <div class="footer-text">built with precision &nbsp;·&nbsp; © hash labs</div>
  </div>

</div>
</body>
</html>
