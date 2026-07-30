<div align="center">

<!-- 3D BANNER -->
<svg viewBox="0 0 860 220" xmlns="http://www.w3.org/2000/svg" width="100%" style="max-width:860px">
  <defs>
    <!-- Deep space background gradient -->
    <linearGradient id="bg" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#060818"/>
      <stop offset="50%" style="stop-color:#0d1225"/>
      <stop offset="100%" style="stop-color:#060818"/>
    </linearGradient>
    <!-- 3D top face of text block -->
    <linearGradient id="topFace" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#7eb8f7"/>
      <stop offset="100%" style="stop-color:#3a7bd5"/>
    </linearGradient>
    <!-- 3D side/shadow face -->
    <linearGradient id="sideFace" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#1a3a6b"/>
      <stop offset="100%" style="stop-color:#0d2147"/>
    </linearGradient>
    <!-- Glow filter for text -->
    <filter id="glow" x="-20%" y="-20%" width="140%" height="140%">
      <feGaussianBlur stdDeviation="3.5" result="coloredBlur"/>
      <feMerge>
        <feMergeNode in="coloredBlur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
    <!-- Soft ambient glow -->
    <filter id="ambientGlow" x="-50%" y="-50%" width="200%" height="200%">
      <feGaussianBlur stdDeviation="18" result="coloredBlur"/>
      <feMerge>
        <feMergeNode in="coloredBlur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
    <!-- Grid line pattern -->
    <pattern id="grid" width="40" height="40" patternUnits="userSpaceOnUse">
      <path d="M 40 0 L 0 0 0 40" fill="none" stroke="#1a2a4a" stroke-width="0.6"/>
    </pattern>
    <!-- Perspective grid bottom gradient -->
    <linearGradient id="gridFade" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#060818;stop-opacity:0"/>
      <stop offset="100%" style="stop-color:#060818;stop-opacity:1"/>
    </linearGradient>
    <!-- Blue radial glow under text -->
    <radialGradient id="centerGlow" cx="50%" cy="60%" r="45%">
      <stop offset="0%" style="stop-color:#2563eb;stop-opacity:0.35"/>
      <stop offset="100%" style="stop-color:#060818;stop-opacity:0"/>
    </radialGradient>
    <!-- Shimmer on top face -->
    <linearGradient id="shimmer" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#ffffff;stop-opacity:0"/>
      <stop offset="45%" style="stop-color:#ffffff;stop-opacity:0.18"/>
      <stop offset="55%" style="stop-color:#ffffff;stop-opacity:0.22"/>
      <stop offset="100%" style="stop-color:#ffffff;stop-opacity:0"/>
    </linearGradient>
    <!-- Reflection gradient -->
    <linearGradient id="reflect" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#3a7bd5;stop-opacity:0.4"/>
      <stop offset="100%" style="stop-color:#3a7bd5;stop-opacity:0"/>
    </linearGradient>
  </defs>

  <!-- Background -->
  <rect width="860" height="220" fill="url(#bg)" rx="14"/>

  <!-- Perspective grid floor -->
  <g opacity="0.55">
    <!-- Converging perspective lines from bottom horizon -->
    <line x1="430" y1="155" x2="0" y2="220" stroke="#1e3a6e" stroke-width="0.7"/>
    <line x1="430" y1="155" x2="86" y2="220" stroke="#1e3a6e" stroke-width="0.7"/>
    <line x1="430" y1="155" x2="172" y2="220" stroke="#1e3a6e" stroke-width="0.7"/>
    <line x1="430" y1="155" x2="258" y2="220" stroke="#1e3a6e" stroke-width="0.7"/>
    <line x1="430" y1="155" x2="344" y2="220" stroke="#1e3a6e" stroke-width="0.7"/>
    <line x1="430" y1="155" x2="430" y2="220" stroke="#1e3a6e" stroke-width="0.7"/>
    <line x1="430" y1="155" x2="516" y2="220" stroke="#1e3a6e" stroke-width="0.7"/>
    <line x1="430" y1="155" x2="602" y2="220" stroke="#1e3a6e" stroke-width="0.7"/>
    <line x1="430" y1="155" x2="688" y2="220" stroke="#1e3a6e" stroke-width="0.7"/>
    <line x1="430" y1="155" x2="774" y2="220" stroke="#1e3a6e" stroke-width="0.7"/>
    <line x1="430" y1="155" x2="860" y2="220" stroke="#1e3a6e" stroke-width="0.7"/>
    <!-- Horizontal cross lines on grid -->
    <line x1="0" y1="175" x2="860" y2="175" stroke="#1e3a6e" stroke-width="0.5"/>
    <line x1="0" y1="192" x2="860" y2="192" stroke="#1e3a6e" stroke-width="0.5"/>
    <line x1="0" y1="207" x2="860" y2="207" stroke="#1e3a6e" stroke-width="0.5"/>
    <line x1="0" y1="220" x2="860" y2="220" stroke="#1e3a6e" stroke-width="0.5"/>
  </g>
  <!-- Fade floor grid at bottom -->
  <rect x="0" y="155" width="860" height="65" fill="url(#gridFade)"/>

  <!-- Center ambient glow -->
  <ellipse cx="430" cy="120" rx="320" ry="80" fill="url(#centerGlow)"/>

  <!-- Floating particles -->
  <circle cx="80"  cy="40"  r="1.5" fill="#58a6ff" opacity="0.7"/>
  <circle cx="200" cy="20"  r="1"   fill="#58a6ff" opacity="0.5"/>
  <circle cx="660" cy="30"  r="1.5" fill="#58a6ff" opacity="0.7"/>
  <circle cx="790" cy="55"  r="1"   fill="#7eb8f7" opacity="0.5"/>
  <circle cx="140" cy="170" r="1"   fill="#3a7bd5" opacity="0.4"/>
  <circle cx="720" cy="160" r="1.2" fill="#3a7bd5" opacity="0.4"/>
  <circle cx="50"  cy="110" r="0.8" fill="#58a6ff" opacity="0.5"/>
  <circle cx="820" cy="100" r="0.8" fill="#58a6ff" opacity="0.5"/>

  <!-- Horizontal accent line -->
  <line x1="60" y1="148" x2="800" y2="148" stroke="#1e3a6e" stroke-width="0.8" opacity="0.8"/>

  <!-- === 3D EXTRUDED MAIN TITLE === -->
  <!-- Shadow layers (extrusion depth) — darkest to lightest -->
  <text x="433" y="96" font-family="'Arial Black',Arial,sans-serif" font-size="54" font-weight="900" fill="#040c1e" text-anchor="middle" letter-spacing="-1">CHITRAJU VISHNU VINEETH</text>
  <text x="432" y="95" font-family="'Arial Black',Arial,sans-serif" font-size="54" font-weight="900" fill="#071635" text-anchor="middle" letter-spacing="-1">CHITRAJU VISHNU VINEETH</text>
  <text x="431" y="94" font-family="'Arial Black',Arial,sans-serif" font-size="54" font-weight="900" fill="#0d2147" text-anchor="middle" letter-spacing="-1">CHITRAJU VISHNU VINEETH</text>
  <text x="430.5" y="93" font-family="'Arial Black',Arial,sans-serif" font-size="54" font-weight="900" fill="#152e60" text-anchor="middle" letter-spacing="-1">CHITRAJU VISHNU VINEETH</text>
  <text x="430" y="92" font-family="'Arial Black',Arial,sans-serif" font-size="54" font-weight="900" fill="#1e3a6e" text-anchor="middle" letter-spacing="-1">CHITRAJU VISHNU VINEETH</text>
  <!-- Main face with glow -->
  <text x="430" y="90" font-family="'Arial Black',Arial,sans-serif" font-size="54" font-weight="900"
    fill="url(#topFace)" text-anchor="middle" letter-spacing="-1" filter="url(#glow)">CHITRAJU VISHNU VINEETH</text>
  <!-- Shimmer overlay -->
  <text x="430" y="90" font-family="'Arial Black',Arial,sans-serif" font-size="54" font-weight="900"
    fill="url(#shimmer)" text-anchor="middle" letter-spacing="-1" opacity="0.6">CHITRAJU VISHNU VINEETH</text>

  <!-- Text reflection below -->
  <text x="430" y="105" font-family="'Arial Black',Arial,sans-serif" font-size="54" font-weight="900"
    fill="url(#reflect)" text-anchor="middle" letter-spacing="-1" transform="scale(1,-1) translate(0,-195)" opacity="0.18">CHITRAJU VISHNU VINEETH</text>

  <!-- === SUBTITLE with 3D depth === -->
  <text x="431" y="127" font-family="Arial,sans-serif" font-size="14" font-weight="400" fill="#0d2147" text-anchor="middle" letter-spacing="5">FULL STACK DEVELOPER  ·  ENGINEERING STUDENT  ·  CHENNAI</text>
  <text x="430" y="126" font-family="Arial,sans-serif" font-size="14" font-weight="400" fill="#7eb8f7" text-anchor="middle" letter-spacing="5" opacity="0.85">FULL STACK DEVELOPER  ·  ENGINEERING STUDENT  ·  CHENNAI</text>

  <!-- Bottom accent bar — glowing line -->
  <rect x="330" y="140" width="200" height="2" rx="1" fill="#3a7bd5" opacity="0.5"/>
  <rect x="380" y="140" width="100" height="2" rx="1" fill="#7eb8f7" opacity="0.9" filter="url(#glow)"/>

  <!-- Corner accents -->
  <path d="M 16 16 L 16 36 M 16 16 L 36 16" stroke="#3a7bd5" stroke-width="1.5" fill="none" opacity="0.7"/>
  <path d="M 844 16 L 844 36 M 844 16 L 824 16" stroke="#3a7bd5" stroke-width="1.5" fill="none" opacity="0.7"/>
  <path d="M 16 204 L 16 184 M 16 204 L 36 204" stroke="#3a7bd5" stroke-width="1.5" fill="none" opacity="0.7"/>
  <path d="M 844 204 L 844 184 M 844 204 L 824 204" stroke="#3a7bd5" stroke-width="1.5" fill="none" opacity="0.7"/>
</svg>

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/chitraju-vishnu-vineeth)
[![Gmail](https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:vishnuvineeth2470039@ssn.edu.in)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/VishnuVineeth14)
![Profile Views](https://komarev.com/ghpvc/?username=VishnuVineeth14&style=for-the-badge&color=0d1117&label=PROFILE+VIEWS)

</div>

---

## About Me

Full-stack developer passionate about building scalable web applications and data-driven solutions. Currently at **SSN College of Engineering, Chennai**, preparing for placements while shipping real projects. I write clean code, think in systems, and am always exploring what's next.

```
📍 Chennai, India          🎓 Engineering Student         🔭 Open to Collaborations
💡 Full Stack Developer    📊 Data Science Enthusiast      🚀 Placement Ready
```

---

## Tech Stack

### Languages

<p>
  <a href="https://github.com/VishnuVineeth14?tab=repositories&language=c">
    <img src="https://img.shields.io/badge/C-00599C?style=for-the-badge&logo=c&logoColor=white" />
  </a>
  <a href="https://github.com/VishnuVineeth14?tab=repositories&language=java">
    <img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" />
  </a>
  <a href="https://github.com/VishnuVineeth14?tab=repositories&language=python">
    <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=ffdd54" />
  </a>
  <a href="https://github.com/VishnuVineeth14?tab=repositories&language=javascript">
    <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" />
  </a>
  <a href="https://github.com/VishnuVineeth14?tab=repositories&language=kotlin">
    <img src="https://img.shields.io/badge/Kotlin-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white" />
  </a>
</p>

### Frontend & Mobile

<p>
  <a href="https://github.com/VishnuVineeth14?tab=repositories&q=react">
    <img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" />
  </a>
  <a href="https://github.com/VishnuVineeth14?tab=repositories&language=html">
    <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" />
  </a>
  <a href="https://github.com/VishnuVineeth14?tab=repositories&language=css">
    <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" />
  </a>
  <a href="https://github.com/VishnuVineeth14?tab=repositories&language=dart">
    <img src="https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white" />
  </a>
  <a href="https://github.com/VishnuVineeth14?tab=repositories&language=dart">
    <img src="https://img.shields.io/badge/Dart-0175C2?style=for-the-badge&logo=dart&logoColor=white" />
  </a>
</p>

### Backend & Databases

<p>
  <a href="https://github.com/VishnuVineeth14?tab=repositories&q=node">
    <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white" />
  </a>
  <a href="https://github.com/VishnuVineeth14?tab=repositories&q=express">
    <img src="https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white" />
  </a>
  <a href="https://github.com/VishnuVineeth14?tab=repositories&q=flask">
    <img src="https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white" />
  </a>
  <a href="https://github.com/VishnuVineeth14?tab=repositories&q=mongodb">
    <img src="https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white" />
  </a>
  <a href="https://github.com/VishnuVineeth14?tab=repositories&q=mysql">
    <img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white" />
  </a>
  <a href="https://github.com/VishnuVineeth14?tab=repositories&q=sqlite">
    <img src="https://img.shields.io/badge/SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white" />
  </a>
  <a href="https://github.com/VishnuVineeth14?tab=repositories&q=neo4j">
    <img src="https://img.shields.io/badge/Neo4j-008CC1?style=for-the-badge&logo=neo4j&logoColor=white" />
  </a>
</p>

### Data Science & ML

<p>
  <a href="https://github.com/VishnuVineeth14?tab=repositories&q=pandas">
    <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" />
  </a>
  <a href="https://github.com/VishnuVineeth14?tab=repositories&q=numpy">
    <img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white" />
  </a>
  <a href="https://github.com/VishnuVineeth14?tab=repositories&q=sklearn">
    <img src="https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white" />
  </a>
  <a href="https://github.com/VishnuVineeth14?tab=repositories&q=tensorflow">
    <img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white" />
  </a>
  <a href="https://github.com/VishnuVineeth14?tab=repositories&q=matplotlib">
    <img src="https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=python&logoColor=white" />
  </a>
</p>

### DevOps & Cloud

<p>
  <a href="https://github.com/VishnuVineeth14?tab=repositories&q=docker">
    <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" />
  </a>
  <a href="https://github.com/VishnuVineeth14?tab=repositories&q=firebase">
    <img src="https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black" />
  </a>
  <a href="https://github.com/VishnuVineeth14?tab=repositories&q=vercel">
    <img src="https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white" />
  </a>
  <a href="https://github.com/VishnuVineeth14?tab=repositories&q=netlify">
    <img src="https://img.shields.io/badge/Netlify-00C7B7?style=for-the-badge&logo=netlify&logoColor=white" />
  </a>
  <a href="https://github.com/VishnuVineeth14?tab=repositories&q=actions">
    <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white" />
  </a>
</p>

---

## Featured Project

<a href="https://github.com/VishnuVineeth14/Mess-Management-Platform">
  <img align="center" src="https://github-readme-stats.vercel.app/api/pin/?username=VishnuVineeth14&repo=Mess-Management-Platform&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=58a6ff&icon_color=58a6ff&text_color=c9d1d9" />
</a>

> Real-time hostel mess operations platform — billing, attendance tracking, and intuitive UI built with **Flutter & Dart**

---

## GitHub Analytics

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=VishnuVineeth14&show_icons=true&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=58a6ff&icon_color=58a6ff&text_color=c9d1d9&cache_seconds=1800" />
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=VishnuVineeth14&layout=compact&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=58a6ff&text_color=c9d1d9&cache_seconds=1800" />

<br/>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/VishnuVineeth14/VishnuVineeth14/main/dist/github-contribution-grid-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/VishnuVineeth14/VishnuVineeth14/main/dist/github-contribution-grid-snake.svg" />
  <img alt="contribution snake" src="https://raw.githubusercontent.com/VishnuVineeth14/VishnuVineeth14/main/dist/github-contribution-grid-snake-dark.svg" width="98%" />
</picture>

</div>

---

<div align="center">

*Open to collaborations · Building in public · Chennai, India*

</div>
