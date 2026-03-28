<!-- ═══════════════════════════════════════════════════════════════ -->
<!--                  ANIMATED HEADER BANNER SVG                     -->
<!-- ═══════════════════════════════════════════════════════════════ -->

<div align="center">

<svg width="860" height="200" viewBox="0 0 860 200" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="bg" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#050508"/>
      <stop offset="100%" style="stop-color:#0d0d1a"/>
    </linearGradient>
    <linearGradient id="textGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#7c5cfc"/>
      <stop offset="50%" style="stop-color:#fc5c7d"/>
      <stop offset="100%" style="stop-color:#56ccf2"/>
    </linearGradient>
    <linearGradient id="lineGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#7c5cfc;stop-opacity:0"/>
      <stop offset="50%" style="stop-color:#7c5cfc"/>
      <stop offset="100%" style="stop-color:#56ccf2;stop-opacity:0"/>
    </linearGradient>
    <filter id="glow">
      <feGaussianBlur stdDeviation="3" result="coloredBlur"/>
      <feMerge><feMergeNode in="coloredBlur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <filter id="glow2">
      <feGaussianBlur stdDeviation="8" result="coloredBlur"/>
      <feMerge><feMergeNode in="coloredBlur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <style>
      .grid-line { stroke: rgba(124,92,252,0.07); stroke-width: 0.5; }
      .dot { fill: rgba(124,92,252,0.4); }
      @keyframes fadeUp { from { opacity:0; transform:translateY(20px); } to { opacity:1; transform:translateY(0); } }
      @keyframes scanX { 0%{transform:translateX(-860px)} 100%{transform:translateX(860px)} }
      @keyframes pulse { 0%,100%{opacity:0.3} 50%{opacity:1} }
      @keyframes blink { 0%,100%{opacity:1} 50%{opacity:0} }
      @keyframes orbit { from{transform:rotate(0deg) translateX(60px) rotate(0deg)} to{transform:rotate(360deg) translateX(60px) rotate(-360deg)} }
      @keyframes float { 0%,100%{transform:translateY(0)} 50%{transform:translateY(-6px)} }
      .name-text { animation: fadeUp 1s ease both; }
      .role-text { animation: fadeUp 1s 0.3s ease both; }
      .scan-line { animation: scanX 4s linear infinite; opacity: 0.15; }
      .orb1 { animation: pulse 3s ease infinite; }
      .orb2 { animation: pulse 4s 1s ease infinite; }
      .cursor-blink { animation: blink 1s step-end infinite; }
      .float-el { animation: float 3s ease-in-out infinite; }
    </style>
  </defs>

  <!-- Background -->
  <rect width="860" height="200" fill="url(#bg)" rx="12"/>

  <!-- Grid lines horizontal -->
  <line x1="0" y1="40" x2="860" y2="40" class="grid-line"/>
  <line x1="0" y1="80" x2="860" y2="80" class="grid-line"/>
  <line x1="0" y1="120" x2="860" y2="120" class="grid-line"/>
  <line x1="0" y1="160" x2="860" y2="160" class="grid-line"/>
  <!-- Grid lines vertical -->
  <line x1="86" y1="0" x2="86" y2="200" class="grid-line"/>
  <line x1="172" y1="0" x2="172" y2="200" class="grid-line"/>
  <line x1="258" y1="0" x2="258" y2="200" class="grid-line"/>
  <line x1="344" y1="0" x2="344" y2="200" class="grid-line"/>
  <line x1="430" y1="0" x2="430" y2="200" class="grid-line"/>
  <line x1="516" y1="0" x2="516" y2="200" class="grid-line"/>
  <line x1="602" y1="0" x2="602" y2="200" class="grid-line"/>
  <line x1="688" y1="0" x2="688" y2="200" class="grid-line"/>
  <line x1="774" y1="0" x2="774" y2="200" class="grid-line"/>

  <!-- Scanning line -->
  <rect class="scan-line" x="0" y="0" width="120" height="200" fill="url(#lineGrad)"/>

  <!-- Glow orbs -->
  <circle class="orb1" cx="720" cy="50" r="80" fill="rgba(124,92,252,0.07)"/>
  <circle class="orb2" cx="780" cy="150" r="60" fill="rgba(86,204,242,0.06)"/>
  <circle cx="100" cy="150" r="50" fill="rgba(252,92,125,0.05)" class="orb1"/>

  <!-- Decorative dots -->
  <circle class="dot" cx="30" cy="30" r="1.5"/>
  <circle class="dot" cx="830" cy="170" r="1.5"/>
  <circle class="dot" cx="430" cy="15" r="1.5"/>
  <circle class="dot" cx="430" cy="185" r="1.5"/>

  <!-- Border glow -->
  <rect width="860" height="200" fill="none" stroke="url(#lineGrad)" stroke-width="1" rx="12" opacity="0.6"/>

  <!-- Top-left tag -->
  <rect x="20" y="18" width="130" height="18" rx="3" fill="rgba(124,92,252,0.15)" stroke="rgba(124,92,252,0.4)" stroke-width="0.8"/>
  <circle cx="33" cy="27" r="4" fill="#43e97b">
    <animate attributeName="opacity" values="1;0.2;1" dur="1.5s" repeatCount="indefinite"/>
  </circle>
  <text x="43" y="31" font-family="monospace" font-size="8" fill="#43e97b" letter-spacing="1">AVAILABLE TO HIRE</text>

  <!-- Main Name -->
  <text class="name-text float-el" x="430" y="90" text-anchor="middle"
    font-family="monospace" font-size="46" font-weight="bold"
    fill="url(#textGrad)" filter="url(#glow2)" letter-spacing="-1">
    SAURABH PRAJAPATI
  </text>

  <!-- Role line -->
  <text class="role-text" x="430" y="120" text-anchor="middle"
    font-family="monospace" font-size="11" fill="rgba(255,255,255,0.45)" letter-spacing="5">
    FULL STACK DEVELOPER  ·  AI ENGINEER  ·  DECODEX7
  </text>

  <!-- Divider line -->
  <line x1="160" y1="133" x2="700" y2="133" stroke="url(#lineGrad)" stroke-width="0.8"/>

  <!-- Bottom stat chips -->
  <!-- .NET -->
  <rect x="155" y="148" width="68" height="20" rx="3" fill="rgba(124,92,252,0.15)" stroke="rgba(124,92,252,0.35)" stroke-width="0.8"/>
  <text x="189" y="162" text-anchor="middle" font-family="monospace" font-size="8" fill="#7c5cfc" letter-spacing="0.5">ASP.NET CORE</text>

  <!-- PostgreSQL -->
  <rect x="231" y="148" width="72" height="20" rx="3" fill="rgba(67,233,123,0.1)" stroke="rgba(67,233,123,0.3)" stroke-width="0.8"/>
  <text x="267" y="162" text-anchor="middle" font-family="monospace" font-size="8" fill="#43e97b" letter-spacing="0.5">MySQL</text>

  <!-- PyTorch -->
  <rect x="311" y="148" width="58" height="20" rx="3" fill="rgba(252,92,125,0.1)" stroke="rgba(252,92,125,0.3)" stroke-width="0.8"/>
  <text x="340" y="162" text-anchor="middle" font-family="monospace" font-size="8" fill="#fc5c7d" letter-spacing="0.5">PYTORCH</text>

  <!-- Docker -->
  <rect x="377" y="148" width="50" height="20" rx="3" fill="rgba(86,204,242,0.1)" stroke="rgba(86,204,242,0.3)" stroke-width="0.8"/>
  <text x="402" y="162" text-anchor="middle" font-family="monospace" font-size="8" fill="#56ccf2" letter-spacing="0.5">DOCKER</text>

  <!-- C# -->
  <rect x="435" y="148" width="36" height="20" rx="3" fill="rgba(124,92,252,0.12)" stroke="rgba(124,92,252,0.3)" stroke-width="0.8"/>
  <text x="453" y="162" text-anchor="middle" font-family="monospace" font-size="8" fill="#7c5cfc" letter-spacing="0.5">C#</text>

  <!-- Python -->
  <rect x="479" y="148" width="52" height="20" rx="3" fill="rgba(247,201,72,0.1)" stroke="rgba(247,201,72,0.3)" stroke-width="0.8"/>
  <text x="505" y="162" text-anchor="middle" font-family="monospace" font-size="8" fill="#f7c948" letter-spacing="0.5">PYTHON</text>

  <!-- EF Core -->
  <rect x="539" y="148" width="50" height="20" rx="3" fill="rgba(67,233,123,0.1)" stroke="rgba(67,233,123,0.3)" stroke-width="0.8"/>
  <text x="564" y="162" text-anchor="middle" font-family="monospace" font-size="8" fill="#43e97b" letter-spacing="0.5">EF CORE</text>

  <!-- Git -->
  <rect x="597" y="148" width="58" height="20" rx="3" fill="rgba(252,92,125,0.1)" stroke="rgba(252,92,125,0.3)" stroke-width="0.8"/>
  <text x="626" y="162" text-anchor="middle" font-family="monospace" font-size="8" fill="#fc5c7d" letter-spacing="0.5">GIT / GITHUB</text>

  <!-- Corner decoration top-right -->
  <line x1="820" y1="20" x2="840" y2="20" stroke="rgba(124,92,252,0.5)" stroke-width="1.5"/>
  <line x1="840" y1="20" x2="840" y2="40" stroke="rgba(124,92,252,0.5)" stroke-width="1.5"/>
  <!-- Corner decoration bottom-left -->
  <line x1="20" y1="180" x2="40" y2="180" stroke="rgba(86,204,242,0.5)" stroke-width="1.5"/>
  <line x1="20" y1="160" x2="20" y2="180" stroke="rgba(86,204,242,0.5)" stroke-width="1.5"/>
</svg>

</div>

<!-- ═══════════════════════════════════════════════════════════════ -->
<!--                    ANIMATED TYPING TEXT                         -->
<!-- ═══════════════════════════════════════════════════════════════ -->

<div align="center">

[![Typing SVG](https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=18&duration=3000&pause=800&color=7C5CFC&center=true&vCenter=true&multiline=false&width=700&lines=🚀+Building+production-grade+web+systems;⚙️+ASP.NET+Core+%7C+PostgreSQL+%7C+EF+Core+8;🧠+Deep+Learning+%7C+ResNet50+%7C+PyTorch;🐳+Docker+%7C+Render+%7C+Cloud+Deployment;💡+Turning+complex+problems+into+clean+code)](https://git.io/typing-svg)

</div>

<br/>

<!-- ═══════════════════════════════════════════════════════════════ -->
<!--                      ABOUT ME SECTION                           -->
<!-- ═══════════════════════════════════════════════════════════════ -->

<img align="right" width="340" src="https://raw.githubusercontent.com/abhisheknaiidu/abhisheknaiidu/master/code.gif" alt="coding gif"/>

### 👋 &nbsp;`whoami`

```yaml
name      : "Saurabh Prajapati"
alias     : "DecodeX7"
degree    : "B.Tech CSE (Artificial Intelligence)"
location  : "Varanasi, India 🇮🇳"
status    : "Open to work → Full-time & Internships"
focus     : ["Full Stack Dev", "AI/ML Engineering", "Data Analyst"]
```

<br/>

🔭 &nbsp;Currently building **Smart Systems** with ASP.NET Core + MySQL  
🧠 &nbsp;Deep Learning enthusiast — **ResNet50**, **Grad-CAM**, **Transfer Learning**  
🐳 &nbsp;Containerizing everything with **Docker** — deployed on **Render**  
⚡ &nbsp;Fun fact: I name all my projects like space missions 🪐  
📫 &nbsp;Reach me on **[Instagram](https://www.instagram.com/s.108.p?igsh=N3NodG5pMHA5eWhv)** or **[GitHub](https://github.com/DecodeX7)**

<br clear="right"/>

---

<!-- ═══════════════════════════════════════════════════════════════ -->
<!--                     TECH STACK SECTION                          -->
<!-- ═══════════════════════════════════════════════════════════════ -->

<h2 align="center">⚡ &nbsp;Tech Arsenal</h2>

<div align="center">

**🖥️ Backend & Frameworks**

[![My Skills](https://skillicons.dev/icons?i=dotnet,cs,python,flask&theme=dark)](https://skillicons.dev)

**🗄️ Databases & ORM**

[![My Skills](https://skillicons.dev/icons?i=postgres,sqlite,mysql&theme=dark)](https://skillicons.dev)

**🤖 AI / Machine Learning**

[![My Skills](https://skillicons.dev/icons?i=pytorch,tensorflow,opencv&theme=dark)](https://skillicons.dev)

**🎨 Frontend**

[![My Skills](https://skillicons.dev/icons?i=html,css,js,bootstrap&theme=dark)](https://skillicons.dev)

**🛠️ DevOps & Tools**

[![My Skills](https://skillicons.dev/icons?i=docker,git,github,vscode,visualstudio,linux&theme=dark)](https://skillicons.dev)

</div>

<br/>

<div align="center">

<!-- Detailed badge row -->
![ASP.NET Core](https://img.shields.io/badge/ASP.NET_Core-MVC-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![.NET 8](https://img.shields.io/badge/.NET-8.0-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![C#](https://img.shields.io/badge/C%23-239120?style=flat-square&logo=csharp&logoColor=white)
![EF Core](https://img.shields.io/badge/EF_Core-8.0.2-6DB33F?style=flat-square)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=flat-square&logo=postgresql&logoColor=white)
![Npgsql](https://img.shields.io/badge/Npgsql-8.0.2-336791?style=flat-square)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Render](https://img.shields.io/badge/Render-000000?style=flat-square&logo=render&logoColor=white)
![BCrypt](https://img.shields.io/badge/BCrypt.Net-4.1.0-red?style=flat-square)
![MailKit](https://img.shields.io/badge/MailKit-4.15.1-orange?style=flat-square)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Bootstrap](https://img.shields.io/badge/Bootstrap-7952B3?style=flat-square&logo=bootstrap&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

</div>

---

<!-- ═══════════════════════════════════════════════════════════════ -->
<!--                    FEATURED PROJECTS                            -->
<!-- ═══════════════════════════════════════════════════════════════ -->

<h2 align="center">🚀 &nbsp;Featured Projects</h2>

<br/>

<!-- ROW 1 -->
<table>
<tr>
<td width="50%" valign="top">

### 🪐 Nova Admin — Multi-Step Form Portal
> **Production-deployed** application portal on Render

A real-world college/government/job application system. Multi-step form (Personal → Qualification → Address → Preview → Submit), PostgreSQL persistence, Admin CRUD dashboard with dynamic JSON education rendering.

**Stack:**
`ASP.NET Core MVC` · `.NET 8` · `PostgreSQL` · `EF Core` · `Docker` · `Razor` · `Bootstrap`

[![Live Demo](https://img.shields.io/badge/🌐_Live_Demo-00C7B7?style=for-the-badge)](https://nova-admin-torz.onrender.com)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github)](https://github.com/DecodeX7/Nova-Admin)
[![YouTube](https://img.shields.io/badge/Demo-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://youtu.be/NQCug-ooOQk)

</td>
<td width="50%" valign="top">

### 🔬 Image Recognition & Fraud Detection
> **Deep Learning** — ResNet50 + Grad-CAM + PyTorch

ResNet50-based classification and fraud/anomaly detection using Transfer Learning. Features Grad-CAM heatmaps for interpretability, misclassification analysis, and an interactive Streamlit UI. Fully Dockerized with modular architecture.

**Stack:**
`PyTorch` · `ResNet50` · `Transfer Learning` · `Grad-CAM` · `Streamlit` · `Docker` · `Python`

[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github)](https://github.com/DecodeX7/Image-Recognition-System-Project)

</td>
</tr>

<tr>
<td width="50%" valign="top">

### 📚 Library Management System
> **Full-featured** library portal with role-based auth

Complete library portal — book catalog, issue/return tracking, automated fine calculation per day, OTP password reset, email notifications via MailKit, BCrypt auth. Dual panels for Admin + Student.

**Stack:**
`ASP.NET Core MVC` · `.NET 8` · `SQL Server` · `EF Core` · `BCrypt` · `MailKit` · `MimeKit`

[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github)](https://github.com/DecodeX7/LibraryManagementSystem)
[![YouTube](https://img.shields.io/badge/Demo-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://youtu.be/RZDayx180Gg)

</td>
<td width="50%" valign="top">

### 📡 Smart Attendance Management System
> **Face-recognition powered** attendance tracker

Python/Flask attendance system with face recognition, SQLite database, CSV export, and live tracking. 55+ commits of active development. Deployed with Procfile for Heroku-style platforms.

**Stack:**
`Python` · `Flask` · `OpenCV` · `SQLite` · `Face Recognition` · `HTML/CSS`

[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github)](https://github.com/DecodeX7/Smart-Attendance-Management-System)

</td>
</tr>

<tr>
<td width="50%" valign="top">

### 🎓 Student CRUD App
> **Containerized** student records management

Clean MVC student management with full CRUD. Multi-stage Docker build keeps image lean. Auto-migrations on startup, PostgreSQL via Npgsql, profile image uploads, Bootstrap UI.

**Stack:**
`ASP.NET Core MVC` · `.NET 8` · `PostgreSQL` · `EF Core 8` · `Docker` · `Npgsql`

[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github)](https://github.com/DecodeX7/StudentCRUD)

</td>
<td width="50%" valign="top">

### 📊 DSA — Data Structures & Algorithms
> **Java** — Core concepts + Algorithm implementations

Comprehensive DSA implementations covering sorting algorithms, trees, graphs, dynamic programming, and more. A structured reference for competitive programming and interview prep.

**Stack:**
`Java` · `Data Structures` · `Algorithms` · `OOP`

[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github)](https://github.com/DecodeX7/DSA)

</td>
</tr>
</table>

<br/>

<div align="center">

[![View All Repos](https://img.shields.io/badge/View_All_25+_Repos-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/DecodeX7?tab=repositories)

</div>

---

<!-- ═══════════════════════════════════════════════════════════════ -->
<!--                     GITHUB STATS                               -->
<!-- ═══════════════════════════════════════════════════════════════ -->

<h2 align="center">📊 &nbsp;GitHub Stats</h2>

<br/>

<div align="center">

<img height="180" src="https://github-readme-stats.vercel.app/api?username=DecodeX7&show_icons=true&theme=midnight-purple&hide_border=true&bg_color=0d0d14&title_color=7c5cfc&icon_color=fc5c7d&text_color=e8e8f0&rank_icon=github&include_all_commits=true&count_private=true" />
&nbsp;&nbsp;
<img height="180" src="https://github-readme-stats.vercel.app/api/top-langs/?username=DecodeX7&layout=compact&theme=midnight-purple&hide_border=true&bg_color=0d0d14&title_color=7c5cfc&text_color=e8e8f0&langs_count=8" />

</div>

<br/>

<div align="center">

<img src="https://github-readme-streak-stats.herokuapp.com?user=DecodeX7&theme=midnight-purple&hide_border=true&background=0d0d14&stroke=7c5cfc&ring=fc5c7d&fire=fc5c7d&currStreakLabel=7c5cfc&sideLabels=e8e8f0&dates=6b6b85&currStreakNum=e8e8f0&sideNums=e8e8f0" />

</div>

<br/>

<!-- Trophy -->
<div align="center">

[![trophy](https://github-profile-trophy.vercel.app/?username=DecodeX7&theme=darkhub&no-frame=true&no-bg=true&margin-w=8&column=7)](https://github.com/ryo-ma/github-profile-trophy)

</div>

---

<!-- ═══════════════════════════════════════════════════════════════ -->
<!--                   CONTRIBUTION GRAPH                            -->
<!-- ═══════════════════════════════════════════════════════════════ -->

<h2 align="center">🐍 &nbsp;Contribution Snake</h2>

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/DecodeX7/DecodeX7/output/github-contribution-grid-snake-dark.svg"/>
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/DecodeX7/DecodeX7/output/github-contribution-grid-snake.svg"/>
  <img alt="github contribution grid snake animation" src="https://raw.githubusercontent.com/DecodeX7/DecodeX7/output/github-contribution-grid-snake-dark.svg"/>
</picture>

> ⚠️ **Note:** For the snake animation, set up the GitHub Action below in your profile repo.

</div>

---

<!-- ═══════════════════════════════════════════════════════════════ -->
<!--              ACTIVITY GRAPH                                     -->
<!-- ═══════════════════════════════════════════════════════════════ -->

<h2 align="center">📈 &nbsp;Activity</h2>

<div align="center">

[![Saurabh's github activity graph](https://github-readme-activity-graph.vercel.app/graph?username=DecodeX7&bg_color=0d0d14&color=7c5cfc&line=fc5c7d&point=56ccf2&area=true&area_color=7c5cfc&hide_border=true&custom_title=Saurabh's+Contribution+Graph)](https://github.com/ashutosh00710/github-readme-activity-graph)

</div>

---

<!-- ═══════════════════════════════════════════════════════════════ -->
<!--                 ANIMATED TERMINAL SECTION                       -->
<!-- ═══════════════════════════════════════════════════════════════ -->

<h2 align="center">💻 &nbsp;In My Terminal</h2>

<div align="center">

```bash
❯ saurabh --status

  ╔══════════════════════════════════════════════════════╗
  ║           DECODEX7 // SAURABH PRAJAPATI              ║
  ╠══════════════════════════════════════════════════════╣
  ║  role      →  Full Stack Developer + AI Engineer     ║
  ║  degree    →  B.Tech CSE (Artificial Intelligence)   ║
  ║  location  →  Varanasi, India                        ║
  ╠══════════════════════════════════════════════════════╣
  ║  primary   →  ASP.NET Core MVC / .NET 8 / C#         ║
  ║  database  →  PostgreSQL / SQL Server / EF Core      ║
  ║  ai_ml     →  PyTorch / ResNet50 / Grad-CAM          ║
  ║  devops    →  Docker / Render / Git / GitHub         ║
  ╠══════════════════════════════════════════════════════╣
  ║  status    →  ● AVAILABLE FOR OPPORTUNITIES          ║
  ║  deploy    →  ● nova-admin-torz.onrender.com LIVE    ║
  ║  repos     →  25+ public repositories                ║
  ╚══════════════════════════════════════════════════════╝
```

</div>

---

<!-- ═══════════════════════════════════════════════════════════════ -->
<!--                  CONNECT / FOOTER SECTION                       -->
<!-- ═══════════════════════════════════════════════════════════════ -->

<h2 align="center">🤝 &nbsp;Let's Connect</h2>

<div align="center">

[![GitHub](https://img.shields.io/badge/GitHub-DecodeX7-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/DecodeX7)
[![Instagram](https://img.shields.io/badge/Instagram-spcool786-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://www.instagram.com/spcool786?igsh=N3NodG5pMHA5eWhv)
[![Live Project](https://img.shields.io/badge/🌐_Live_Project-Nova_Admin-00C7B7?style=for-the-badge)](https://nova-admin-torz.onrender.com)

</div>

<br/>

<!-- Footer SVG -->
<div align="center">

<svg width="860" height="60" viewBox="0 0 860 60" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="fg" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#7c5cfc;stop-opacity:0"/>
      <stop offset="30%" style="stop-color:#7c5cfc"/>
      <stop offset="70%" style="stop-color:#fc5c7d"/>
      <stop offset="100%" style="stop-color:#56ccf2;stop-opacity:0"/>
    </linearGradient>
    <style>
      @keyframes wavePulse { 0%,100%{opacity:0.4} 50%{opacity:1} }
      .wave { animation: wavePulse 3s ease infinite; }
    </style>
  </defs>
  <rect width="860" height="60" fill="#050508" rx="0"/>
  <line x1="0" y1="1" x2="860" y2="1" stroke="url(#fg)" stroke-width="1" class="wave"/>
  <text x="430" y="38" text-anchor="middle" font-family="monospace" font-size="11"
    fill="rgba(255,255,255,0.3)" letter-spacing="3">
    © 2025 SAURABH PRAJAPATI  ·  DECODEX7  ·  VARANASI, INDIA
  </text>
  <text x="430" y="54" text-anchor="middle" font-family="monospace" font-size="8"
    fill="rgba(124,92,252,0.5)" letter-spacing="2">
    BUILT WITH PASSION · DEPLOYED WITH DOCKER · POWERED BY COFFEE ☕
  </text>
</svg>

</div>

<div align="center">

![Profile Views](https://komarev.com/ghpvc/?username=DecodeX7&color=7c5cfc&style=flat-square&label=PROFILE+VIEWS)

</div>

---

<!-- ═══════════════════════════════════════════════════════════════ -->
<!--              SETUP INSTRUCTIONS (remove before publish)         -->
<!-- ═══════════════════════════════════════════════════════════════ -->

<details>
<summary>⚙️ <strong>Setup Instructions — Read Before Publishing</strong></summary>

<br/>

### 1. Create your Profile Repository
- Create a **new repo** named exactly `DecodeX7` (same as your username)
- Add this file as `README.md` in the root

### 2. Enable the Snake Animation
Create `.github/workflows/snake.yml` in the `DecodeX7` repo:

```yaml
name: Generate Snake

on:
  schedule:
    - cron: "0 */12 * * *"
  workflow_dispatch:

jobs:
  generate:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      - uses: Platane/snk@v3
        with:
          github_user_name: DecodeX7
          outputs: |
            dist/github-contribution-grid-snake.svg
            dist/github-contribution-grid-snake-dark.svg?palette=github-dark
      - uses: crazy-max/ghaction-github-pages@v3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### 3. What Works Out of the Box
- ✅ Animated SVG header banner
- ✅ Typing animation (readme-typing-svg)
- ✅ Skill icons (skillicons.dev)
- ✅ GitHub Stats, Streak, Top Languages
- ✅ Trophy board
- ✅ Activity graph
- ✅ All project links & badges
- ✅ Terminal-style about block
- ✅ Footer SVG

### 4. After snake workflow runs once
- Remove the `⚠️ Note` line under the snake section
- The snake will auto-update every 12 hours

</details>
