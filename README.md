<div align="center">

<svg width="900" height="200" viewBox="0 0 900 200" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="bg" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#0d0f1a"/>
      <stop offset="100%" style="stop-color:#1a1040"/>
    </linearGradient>
    <linearGradient id="textGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#ffffff"/>
      <stop offset="50%" style="stop-color:#a78bfa"/>
      <stop offset="100%" style="stop-color:#00d4ff"/>
    </linearGradient>
    <linearGradient id="lineGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#6c63ff;stop-opacity:0"/>
      <stop offset="50%" style="stop-color:#6c63ff;stop-opacity:0.8"/>
      <stop offset="100%" style="stop-color:#00d4ff;stop-opacity:0"/>
    </linearGradient>
    <filter id="glow">
      <feGaussianBlur stdDeviation="3" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
  </defs>

  <!-- Background -->
  <rect width="900" height="200" fill="url(#bg)" rx="16"/>

  <!-- Grid lines -->
  <g opacity="0.08">
    <line x1="0" y1="50" x2="900" y2="50" stroke="#6c63ff" stroke-width="0.5"/>
    <line x1="0" y1="100" x2="900" y2="100" stroke="#6c63ff" stroke-width="0.5"/>
    <line x1="0" y1="150" x2="900" y2="150" stroke="#6c63ff" stroke-width="0.5"/>
    <line x1="150" y1="0" x2="150" y2="200" stroke="#6c63ff" stroke-width="0.5"/>
    <line x1="300" y1="0" x2="300" y2="200" stroke="#6c63ff" stroke-width="0.5"/>
    <line x1="450" y1="0" x2="450" y2="200" stroke="#6c63ff" stroke-width="0.5"/>
    <line x1="600" y1="0" x2="600" y2="200" stroke="#6c63ff" stroke-width="0.5"/>
    <line x1="750" y1="0" x2="750" y2="200" stroke="#6c63ff" stroke-width="0.5"/>
  </g>

  <!-- Orb glow left -->
  <circle cx="100" cy="100" r="80" fill="#6c63ff" opacity="0.06">
    <animate attributeName="r" values="80;95;80" dur="4s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.06;0.1;0.06" dur="4s" repeatCount="indefinite"/>
  </circle>

  <!-- Orb glow right -->
  <circle cx="800" cy="100" r="70" fill="#00d4ff" opacity="0.05">
    <animate attributeName="r" values="70;85;70" dur="5s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.05;0.09;0.05" dur="5s" repeatCount="indefinite"/>
  </circle>

  <!-- Hash icon badge -->
  <rect x="30" y="75" width="50" height="50" rx="12" fill="#6c63ff" opacity="0.9">
    <animate attributeName="opacity" values="0.9;1;0.9" dur="3s" repeatCount="indefinite"/>
  </rect>
  <text x="55" y="108" font-family="monospace" font-size="24" font-weight="700" fill="white" text-anchor="middle">#</text>

  <!-- Main title -->
  <text x="450" y="90" font-family="'Segoe UI', sans-serif" font-size="42" font-weight="800"
        fill="url(#textGrad)" text-anchor="middle" filter="url(#glow)">
    Hash Labs
    <animate attributeName="opacity" values="0;1" dur="1s" fill="freeze"/>
  </text>

  <!-- Subtitle -->
  <text x="450" y="120" font-family="monospace" font-size="11" fill="#7c6aff"
        text-anchor="middle" letter-spacing="4">
    ENGINEERING DIGITAL PRODUCTS THAT MATTER
    <animate attributeName="opacity" values="0;1" dur="1.5s" fill="freeze"/>
  </text>

  <!-- Animated line -->
  <line x1="150" y1="140" x2="750" y2="140" stroke="url(#lineGrad)" stroke-width="1">
    <animate attributeName="opacity" values="0;1;0.6" dur="2s" fill="freeze"/>
  </line>

  <!-- Moving particle on line -->
  <circle cx="150" cy="140" r="3" fill="#ffffff" filter="url(#glow)">
    <animate attributeName="cx" values="150;750;150" dur="4s" repeatCount="indefinite" calcMode="spline" keySplines="0.4 0 0.6 1; 0.4 0 0.6 1"/>
    <animate attributeName="opacity" values="0;1;1;0" dur="4s" repeatCount="indefinite"/>
  </circle>

  <!-- Social badges -->
  <rect x="310" y="155" width="130" height="28" rx="14" fill="rgba(228,64,95,0.15)" stroke="#e4405f" stroke-width="0.8">
    <animate attributeName="opacity" values="0;1" dur="2s" fill="freeze"/>
  </rect>
  <text x="375" y="174" font-family="monospace" font-size="11" fill="#e4405f" text-anchor="middle">⬤ @hashc_oding</text>

  <rect x="460" y="155" width="130" height="28" rx="14" fill="rgba(59,130,246,0.15)" stroke="#3b82f6" stroke-width="0.8">
    <animate attributeName="opacity" values="0;1" dur="2.5s" fill="freeze"/>
  </rect>
  <text x="525" y="174" font-family="monospace" font-size="11" fill="#3b82f6" text-anchor="middle">⬤ Hash Company</text>

  <!-- Corner dots decoration -->
  <circle cx="870" cy="20" r="3" fill="#6c63ff" opacity="0.5"><animate attributeName="opacity" values="0.5;1;0.5" dur="2s" repeatCount="indefinite"/></circle>
  <circle cx="860" cy="20" r="2" fill="#6c63ff" opacity="0.3"><animate attributeName="opacity" values="0.3;0.8;0.3" dur="2s" begin="0.3s" repeatCount="indefinite"/></circle>
  <circle cx="850" cy="20" r="1.5" fill="#6c63ff" opacity="0.2"><animate attributeName="opacity" values="0.2;0.6;0.2" dur="2s" begin="0.6s" repeatCount="indefinite"/></circle>
</svg>


</div>

---

## 🧩 ABOUT &nbsp;—&nbsp; Who We Are

**Hash Labs** is a software company that builds digital products for businesses demanding reliability and precision. We specialize in custom web applications, POS systems, and mobile apps — engineered from the ground up with performance-first architecture and clean, maintainable code.

> *"We don't just write code — we engineer systems."*

---

## 🔧 PRODUCTS &nbsp;—&nbsp; What We Build

<div align="center">
<table>
<tr>
<td align="center" width="33%"><b>🌐 Web Applications</b><br/><sub>Scalable, modern platforms built for speed and usability — from dashboards to full SaaS products.</sub></td>
<td align="center" width="33%"><b>🖥️ POS Systems</b><br/><sub>Purpose-built point-of-sale for Pharmacy and Retail — inventory, billing, and reporting in one system.</sub></td>
<td align="center" width="33%"><b>📱 Mobile Apps</b><br/><sub>Cross-platform mobile applications that are fast, intuitive, and ready for production.</sub></td>
</tr>
</table>
</div>

---

## ⚙️ STACK &nbsp;—&nbsp; Tech Stack

<svg width="900" height="120" viewBox="0 0 900 120" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="bg2" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#0d0f1a"/>
      <stop offset="100%" style="stop-color:#0f0d1a"/>
    </linearGradient>
  </defs>
  <rect width="900" height="120" fill="url(#bg2)" rx="12"/>

  <!-- Backend label -->
  <text x="30" y="28" font-family="monospace" font-size="9" fill="#4b5563" letter-spacing="2">BACKEND</text>
  <!-- Laravel -->
  <rect x="30" y="36" width="90" height="28" rx="14" fill="#1a0a0a" stroke="#FF2D20" stroke-width="0.8">
    <animate attributeName="opacity" values="0;1" dur="0.5s" fill="freeze"/>
  </rect>
  <circle cx="46" cy="50" r="4" fill="#FF2D20"/>
  <text x="56" y="55" font-family="monospace" font-size="11" fill="#e2e8f0">Laravel</text>
  <!-- PHP -->
  <rect x="130" y="36" width="70" height="28" rx="14" fill="#1a0a1a" stroke="#777BB4" stroke-width="0.8">
    <animate attributeName="opacity" values="0;1" dur="0.7s" fill="freeze"/>
  </rect>
  <circle cx="146" cy="50" r="4" fill="#777BB4"/>
  <text x="156" y="55" font-family="monospace" font-size="11" fill="#e2e8f0">PHP</text>
  <!-- Node -->
  <rect x="210" y="36" width="90" height="28" rx="14" fill="#0a1a0a" stroke="#339933" stroke-width="0.8">
    <animate attributeName="opacity" values="0;1" dur="0.9s" fill="freeze"/>
  </rect>
  <circle cx="226" cy="50" r="4" fill="#339933"/>
  <text x="236" y="55" font-family="monospace" font-size="11" fill="#e2e8f0">Node.js</text>

  <!-- Frontend label -->
  <text x="330" y="28" font-family="monospace" font-size="9" fill="#4b5563" letter-spacing="2">FRONTEND</text>
  <!-- Next.js -->
  <rect x="330" y="36" width="82" height="28" rx="14" fill="#111111" stroke="#ffffff" stroke-width="0.8" stroke-opacity="0.4">
    <animate attributeName="opacity" values="0;1" dur="1.1s" fill="freeze"/>
  </rect>
  <circle cx="346" cy="50" r="4" fill="#ffffff"/>
  <text x="356" y="55" font-family="monospace" font-size="11" fill="#e2e8f0">Next.js</text>
  <!-- React -->
  <rect x="422" y="36" width="72" height="28" rx="14" fill="#0a1520" stroke="#61DAFB" stroke-width="0.8">
    <animate attributeName="opacity" values="0;1" dur="1.3s" fill="freeze"/>
  </rect>
  <circle cx="438" cy="50" r="4" fill="#61DAFB"/>
  <text x="448" y="55" font-family="monospace" font-size="11" fill="#e2e8f0">React</text>
  <!-- TypeScript -->
  <rect x="504" y="36" width="100" height="28" rx="14" fill="#0a0f20" stroke="#3178C6" stroke-width="0.8">
    <animate attributeName="opacity" values="0;1" dur="1.5s" fill="freeze"/>
  </rect>
  <circle cx="520" cy="50" r="4" fill="#3178C6"/>
  <text x="530" y="55" font-family="monospace" font-size="11" fill="#e2e8f0">TypeScript</text>
  <!-- Tailwind -->
  <rect x="614" y="36" width="106" height="28" rx="14" fill="#0a1520" stroke="#06B6D4" stroke-width="0.8">
    <animate attributeName="opacity" values="0;1" dur="1.7s" fill="freeze"/>
  </rect>
  <circle cx="630" cy="50" r="4" fill="#06B6D4"/>
  <text x="640" y="55" font-family="monospace" font-size="11" fill="#e2e8f0">Tailwind CSS</text>

  <!-- DB label -->
  <text x="30" y="90" font-family="monospace" font-size="9" fill="#4b5563" letter-spacing="2">DATABASE &amp; INFRA</text>
  <!-- PostgreSQL -->
  <rect x="30" y="98" width="110" height="28" rx="14" fill="#0a1020" stroke="#336791" stroke-width="0.8">
    <animate attributeName="opacity" values="0;1" dur="1.9s" fill="freeze"/>
  </rect>
  <circle cx="46" cy="112" r="4" fill="#336791"/>
  <text x="56" y="117" font-family="monospace" font-size="11" fill="#e2e8f0">PostgreSQL</text>
  <!-- MySQL -->
  <rect x="150" y="98" width="78" height="28" rx="14" fill="#0a1020" stroke="#4479A1" stroke-width="0.8">
    <animate attributeName="opacity" values="0;1" dur="2.1s" fill="freeze"/>
  </rect>
  <circle cx="166" cy="112" r="4" fill="#4479A1"/>
  <text x="176" y="117" font-family="monospace" font-size="11" fill="#e2e8f0">MySQL</text>
  <!-- Redis -->
  <rect x="238" y="98" width="72" height="28" rx="14" fill="#1a0a0a" stroke="#DC382D" stroke-width="0.8">
    <animate attributeName="opacity" values="0;1" dur="2.3s" fill="freeze"/>
  </rect>
  <circle cx="254" cy="112" r="4" fill="#DC382D"/>
  <text x="264" y="117" font-family="monospace" font-size="11" fill="#e2e8f0">Redis</text>
  <!-- Docker -->
  <rect x="320" y="98" width="80" height="28" rx="14" fill="#0a1520" stroke="#2496ED" stroke-width="0.8">
    <animate attributeName="opacity" values="0;1" dur="2.5s" fill="freeze"/>
  </rect>
  <circle cx="336" cy="112" r="4" fill="#2496ED"/>
  <text x="346" y="117" font-family="monospace" font-size="11" fill="#e2e8f0">Docker</text>

  <!-- Mobile label -->
  <text x="440" y="90" font-family="monospace" font-size="9" fill="#4b5563" letter-spacing="2">MOBILE</text>
  <!-- React Native -->
  <rect x="440" y="98" width="114" height="28" rx="14" fill="#0a1520" stroke="#61DAFB" stroke-width="0.8">
    <animate attributeName="opacity" values="0;1" dur="2.7s" fill="freeze"/>
  </rect>
  <circle cx="456" cy="112" r="4" fill="#61DAFB"/>
  <text x="466" y="117" font-family="monospace" font-size="11" fill="#e2e8f0">React Native</text>
  <!-- Flutter -->
  <rect x="564" y="98" width="82" height="28" rx="14" fill="#0a1020" stroke="#54C5F8" stroke-width="0.8">
    <animate attributeName="opacity" values="0;1" dur="2.9s" fill="freeze"/>
  </rect>
  <circle cx="580" cy="112" r="4" fill="#54C5F8"/>
  <text x="590" y="117" font-family="monospace" font-size="11" fill="#e2e8f0">Flutter</text>
</svg>


---

## 🎯 FOCUS &nbsp;—&nbsp; Current Focus

<svg width="900" height="160" viewBox="0 0 900 160" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="focusBg" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#0f0d1a"/>
      <stop offset="100%" style="stop-color:#0d1520"/>
    </linearGradient>
    <linearGradient id="accentLine" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#6c63ff"/>
      <stop offset="100%" style="stop-color:#00d4ff"/>
    </linearGradient>
    <filter id="softGlow">
      <feGaussianBlur stdDeviation="2" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
  </defs>

  <rect width="900" height="160" fill="url(#focusBg)" rx="14" stroke="#6c63ff" stroke-width="0.8" stroke-opacity="0.3"/>

  <!-- Glowing left accent bar -->
  <rect x="0" y="0" width="4" height="160" fill="url(#accentLine)" rx="2" filter="url(#softGlow)"/>

  <!-- Pulsing orb top-right -->
  <circle cx="850" cy="40" r="50" fill="#6c63ff" opacity="0.06">
    <animate attributeName="r" values="50;65;50" dur="4s" repeatCount="indefinite"/>
  </circle>

  <!-- Rocket + Title -->
  <text x="28" y="48" font-size="22">🚀</text>
  <text x="58" y="48" font-family="'Segoe UI', sans-serif" font-size="20" font-weight="700" fill="#ffffff" filter="url(#softGlow)">Pharmacy POS System</text>

  <!-- Stack line -->
  <text x="28" y="72" font-family="monospace" font-size="11" fill="#6c63ff">Laravel</text>
  <text x="84" y="72" font-family="monospace" font-size="11" fill="#475569"> · </text>
  <text x="96" y="72" font-family="monospace" font-size="11" fill="#6c63ff">Next.js</text>
  <text x="144" y="72" font-family="monospace" font-size="11" fill="#475569"> · </text>
  <text x="156" y="72" font-family="monospace" font-size="11" fill="#6c63ff">PostgreSQL</text>
  <text x="240" y="72" font-family="monospace" font-size="11" fill="#475569"> — Production-grade, not a prototype.</text>

  <!-- Divider -->
  <line x1="28" y1="84" x2="872" y2="84" stroke="#1e2330" stroke-width="1"/>

  <!-- Features col 1 -->
  <circle cx="38" cy="104" r="3" fill="#6c63ff" filter="url(#softGlow)"><animate attributeName="opacity" values="1;0.4;1" dur="3s" repeatCount="indefinite"/></circle>
  <text x="50" y="109" font-family="'Segoe UI', sans-serif" font-size="12" fill="#94a3b8">Inventory &amp; stock expiry tracking</text>

  <circle cx="38" cy="124" r="3" fill="#6c63ff" filter="url(#softGlow)"><animate attributeName="opacity" values="1;0.4;1" dur="3s" begin="0.5s" repeatCount="indefinite"/></circle>
  <text x="50" y="129" font-family="'Segoe UI', sans-serif" font-size="12" fill="#94a3b8">Supplier &amp; purchase order management</text>

  <circle cx="38" cy="144" r="3" fill="#6c63ff" filter="url(#softGlow)"><animate attributeName="opacity" values="1;0.4;1" dur="3s" begin="1s" repeatCount="indefinite"/></circle>
  <text x="50" y="149" font-family="'Segoe UI', sans-serif" font-size="12" fill="#94a3b8">Customer profiles &amp; purchase history</text>

  <!-- Features col 2 -->
  <circle cx="468" cy="104" r="3" fill="#00d4ff" filter="url(#softGlow)"><animate attributeName="opacity" values="1;0.4;1" dur="3s" begin="0.3s" repeatCount="indefinite"/></circle>
  <text x="480" y="109" font-family="'Segoe UI', sans-serif" font-size="12" fill="#94a3b8">Billing, invoicing &amp; receipt printing</text>

  <circle cx="468" cy="124" r="3" fill="#00d4ff" filter="url(#softGlow)"><animate attributeName="opacity" values="1;0.4;1" dur="3s" begin="0.8s" repeatCount="indefinite"/></circle>
  <text x="480" y="129" font-family="'Segoe UI', sans-serif" font-size="12" fill="#94a3b8">Sales analytics &amp; reporting dashboard</text>

  <circle cx="468" cy="144" r="3" fill="#00d4ff" filter="url(#softGlow)"><animate attributeName="opacity" values="1;0.4;1" dur="3s" begin="1.3s" repeatCount="indefinite"/></circle>
  <text x="480" y="149" font-family="'Segoe UI', sans-serif" font-size="12" fill="#94a3b8">Role-based access control</text>
</svg>


---

## 🧠 MINDSET &nbsp;—&nbsp; How We Think

<svg width="900" height="140" viewBox="0 0 900 140" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="mbg" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#0d0f1a"/>
      <stop offset="100%" style="stop-color:#0f0d1a"/>
    </linearGradient>
  </defs>

  <!-- Card 1 -->
  <rect x="0" y="0" width="218" height="130" rx="12" fill="#0f1219" stroke="#1e2330" stroke-width="1">
    <animate attributeName="stroke-opacity" values="1;0.4;1" dur="4s" repeatCount="indefinite"/>
  </rect>
  <text x="18" y="28" font-family="monospace" font-size="12" fill="#00d4ff">// clean_code</text>
  <line x1="18" y1="36" x2="200" y2="36" stroke="#1e2330" stroke-width="0.8"/>
  <text x="18" y="56" font-family="'Segoe UI', sans-serif" font-size="12" fill="#64748b">No shortcuts. Readable,</text>
  <text x="18" y="74" font-family="'Segoe UI', sans-serif" font-size="12" fill="#64748b">maintainable architecture</text>
  <text x="18" y="92" font-family="'Segoe UI', sans-serif" font-size="12" fill="#64748b">is non-negotiable.</text>

  <!-- Card 2 -->
  <rect x="228" y="0" width="218" height="130" rx="12" fill="#0f1219" stroke="#1e2330" stroke-width="1">
    <animate attributeName="stroke-opacity" values="1;0.4;1" dur="4s" begin="0.5s" repeatCount="indefinite"/>
  </rect>
  <text x="246" y="28" font-family="monospace" font-size="12" fill="#00d4ff">// systems_thinking</text>
  <line x1="246" y1="36" x2="428" y2="36" stroke="#1e2330" stroke-width="0.8"/>
  <text x="246" y="56" font-family="'Segoe UI', sans-serif" font-size="12" fill="#64748b">We design for scale from</text>
  <text x="246" y="74" font-family="'Segoe UI', sans-serif" font-size="12" fill="#64748b">day one — not as an</text>
  <text x="246" y="92" font-family="'Segoe UI', sans-serif" font-size="12" fill="#64748b">afterthought.</text>

  <!-- Card 3 -->
  <rect x="456" y="0" width="218" height="130" rx="12" fill="#0f1219" stroke="#1e2330" stroke-width="1">
    <animate attributeName="stroke-opacity" values="1;0.4;1" dur="4s" begin="1s" repeatCount="indefinite"/>
  </rect>
  <text x="474" y="28" font-family="monospace" font-size="12" fill="#00d4ff">// ship_it</text>
  <line x1="474" y1="36" x2="656" y2="36" stroke="#1e2330" stroke-width="0.8"/>
  <text x="474" y="56" font-family="'Segoe UI', sans-serif" font-size="12" fill="#64748b">Ideas are nothing without</text>
  <text x="474" y="74" font-family="'Segoe UI', sans-serif" font-size="12" fill="#64748b">execution. We build and</text>
  <text x="474" y="92" font-family="'Segoe UI', sans-serif" font-size="12" fill="#64748b">we deliver.</text>

  <!-- Card 4 -->
  <rect x="684" y="0" width="216" height="130" rx="12" fill="#0f1219" stroke="#1e2330" stroke-width="1">
    <animate attributeName="stroke-opacity" values="1;0.4;1" dur="4s" begin="1.5s" repeatCount="indefinite"/>
  </rect>
  <text x="702" y="28" font-family="monospace" font-size="12" fill="#00d4ff">// always_improving</text>
  <line x1="702" y1="36" x2="882" y2="36" stroke="#1e2330" stroke-width="0.8"/>
  <text x="702" y="56" font-family="'Segoe UI', sans-serif" font-size="12" fill="#64748b">Every sprint is a chance</text>
  <text x="702" y="74" font-family="'Segoe UI', sans-serif" font-size="12" fill="#64748b">to do it better than</text>
  <text x="702" y="92" font-family="'Segoe UI', sans-serif" font-size="12" fill="#64748b">the last.</text>
</svg>


---

## 🔗 CONNECT &nbsp;—&nbsp; Follow Us

Stay updated with what we're shipping.

<div align="center">

[![Instagram](https://img.shields.io/badge/-%40hashc__oding-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://instagram.com/hashc_oding)
&nbsp;&nbsp;
[![LinkedIn](https://img.shields.io/badge/-Hash%20Company-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/company/hash-company)

</div>

<br/>

<svg width="900" height="80" viewBox="0 0 900 80" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="fbg" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#0d0f1a"/>
      <stop offset="100%" style="stop-color:#1a1040"/>
    </linearGradient>
    <linearGradient id="fline" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#6c63ff;stop-opacity:0"/>
      <stop offset="50%" style="stop-color:#6c63ff;stop-opacity:0.6"/>
      <stop offset="100%" style="stop-color:#00d4ff;stop-opacity:0"/>
    </linearGradient>
  </defs>
  <rect width="900" height="80" fill="url(#fbg)" rx="12"/>
  <line x1="0" y1="0" x2="900" y2="0" stroke="url(#fline)" stroke-width="1"/>
  <text x="450" y="46" font-family="monospace" font-size="11" fill="#4b5563" text-anchor="middle" letter-spacing="3">
    built with precision  •  © Hash Labs
  </text>
  <!-- Moving dot -->
  <circle cx="0" cy="0" r="2" fill="#6c63ff" opacity="0.8">
    <animateMotion dur="5s" repeatCount="indefinite" path="M0,0 L900,0"/>
    <animate attributeName="opacity" values="0;0.8;0" dur="5s" repeatCount="indefinite"/>
  </circle>
</svg>
