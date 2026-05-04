<html lang="fr">
<head>
<meta charset="UTF-8">
<title>Portfolio — Guendouz Souleyman</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="description" content="Portfolio BTS SIO SISR de Guendouz Souleyman - Administrateur systèmes et réseaux">

<link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@400;500;700&family=JetBrains+Mono:wght@400;600&display=swap" rel="stylesheet">

<style>
:root{
--blue:#00aaff;
--bg:#0d0d0f;
--bg2:#15151b;
--text:#f0f0f0;
--muted:#8c8c95;
--border:rgba(255,255,255,.08);
}
*{margin:0;padding:0;box-sizing:border-box}
body{
font-family:'Space Grotesk',sans-serif;
background:var(--bg);
color:var(--text);
line-height:1.6;
}
a{color:inherit;text-decoration:none}
nav{
position:fixed;top:0;left:0;right:0;
height:64px;
display:flex;justify-content:space-between;align-items:center;
padding:0 30px;
background:rgba(13,13,15,.9);
backdrop-filter:blur(10px);
border-bottom:1px solid var(--border);
z-index:1000;
}
nav .logo{color:var(--blue);font-family:'JetBrains Mono'}
nav ul{display:flex;gap:20px;list-style:none}
nav ul a{color:var(--muted);font-size:.9em}
nav ul a:hover{color:var(--text)}

header{
min-height:100vh;
display:flex;align-items:center;justify-content:center;
text-align:center;
padding:120px 20px;
background:
linear-gradient(rgba(13,13,15,.85),rgba(13,13,15,.95)),
url("https://www.fond-ecran-hd.net/Public/uploads/2019-01-14/thumbs-1/1397.jpg") center/cover;
}
header h1{font-size:clamp(2.5rem,6vw,4.5rem)}
header h1 span{color:var(--blue)}
header p{max-width:650px;margin:20px auto;color:var(--muted)}

section{max-width:1100px;margin:auto;padding:80px 20px}
.section-label{
color:var(--blue);
font-family:'JetBrains Mono';
font-size:.75em;
letter-spacing:.1em;
margin-bottom:10px;
}
h2{font-size:2.2rem;margin-bottom:30px}

.card,.project{
background:var(--bg2);
border:1px solid var(--border);
border-radius:16px;
padding:24px;
margin-bottom:20px;
}
.projects-grid{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(320px,1fr));
gap:20px;
}
ul{margin:10px 0 0 18px;color:var(--muted)}
.tag{
display:inline-block;
margin:6px 6px 0 0;
padding:4px 10px;
border:1px solid rgba(0,170,255,.3);
border-radius:20px;
color:var(--blue);
font-size:.7em;
font-family:'JetBrains Mono';
}
.button{
display:inline-block;
margin-top:14px;
padding:10px 18px;
border-radius:8px;
border:1px solid var(--border);
}
.button:hover{border-color:var(--blue)}

footer{
text-align:center;
padding:30px;
border-top:1px solid var(--border);
color:var(--muted);
font-family:'JetBrains Mono';
}
</style>
</head>

<body>

<nav>
  <div class="logo">GS.dev</div>
  <ul>
    <li><a href="#about">À propos</a></li>
    <li><a href="#parcours">Parcours</a></li>
    <li><a href="#projects">Projets</a></li>
    <li><a href="#veille">Veille</a></li>
    <li><a href="#e6">E6</a></li>
    <li><a href="#contact">Contact</a></li>
  </ul>
</nav>

<header>
  <div>
    <h1>Guendouz<br><span>Souleyman</span></h1>
    <p>
      Étudiant en BTS SIO option SISR à l’IMIE Paris,
      en alternance au Ministère de l’Intérieur.
    </p>
  </div>
</header>

<section id="about">
  <div class="section-label">Profil</div>
  <h2>À propos de moi</h2>
  <div class="card">
    <p>
      Étudiant en BTS SIO option SISR, je me spécialise dans l’administration
      des systèmes et réseaux, la sécurité informatique et la gestion
      d’infrastructures.
    </p>
    <p style="margin-top:10px;">
      <strong>Objectif :</strong> poursuivre en Bachelor ASRC (Administrateur
      Systèmes, Réseaux et Cybersécurité) puis intégrer une entreprise en tant
      qu’administrateur systèmes et réseaux.
    </p>
  </div>
</section>

<section id="parcours">
  <div class="section-label">Parcours</div>
  <h2>Mon parcours</h2>
  <div class="card">
    <strong>BTS SIO SISR — IMIE Paris</strong><br>
    Septembre 2024 → Août 2026
  </div>
  <div class="card">
    <strong>Alternance — Ministère de l’Intérieur</strong>
    <ul>
      <li>Déploiement automatisé de postes (masterisation)</li>
      <li>Installation et configuration de postes</li>
      <li>Support et maintenance du parc</li>
      <li>Gestion Active Directory</li>
      <li>Bêta‑test WAPT & serveur mail</li>
    </ul>
  </div>
</section>

<section id="projects">
  <div class="section-label">Projets</div>
  <h2>Mes projets</h2>

  <div class="projects-grid">

    <div class="project">
      <h3>Serveur Active Directory</h3>
      <p>Contrôleur de domaine Windows Server 2022 (AD, DNS, DHCP, GPO, WDS).</p>
      <a class="button" href="doc-ad.pdf" target="_blank">📄 Documentation</a>
    </div>

    <div class="project">
      <h3>GLPI & FusionInventory</h3>
      <p>Gestion de parc, tickets, SLA, LDAP, inventaire automatique.</p>
      <a class="button" href="projet-glpi.pdf" target="_blank">📄 Documentation</a>
    </div>

    <div class="project">
      <h3>pfSense</h3>
      <p>Pare-feu, NAT, DHCP, segmentation réseau LAN/WAN.</p>
      <a class="button" href="doc-pfsense.pdf" target="_blank">📄 Documentation</a>
    </div>

    <div class="project">
      <h3>Heartbeat</h3>
      <p>Haute disponibilité et failover sous Linux.</p>
      <a class="button" href="tp-heartbeat.pdf" target="_blank">📄 Documentation</a>
    </div>

    <div class="project">
      <h3>Asterisk (VoIP)</h3>
      <p>Serveur VoIP, SIP/PJSIP, extensions, dialplan.</p>
      <a class="button" href="TP-Asterisk-cl.pdf" target="_blank">📄 Documentation</a>
    </div>

  </div>
</section>

<section id="veille">
  <div class="section-label">Veille</div>
  <h2>Veille technologique — Cybersécurité</h2>
  <div class="card">
    <p>
      Veille sur la cybersécurité des systèmes et réseaux :
      menaces, protection des infrastructures, sécurisation AD,
      pare-feux, analyse des logs.
    </p>
  </div>
</section>

<section id="e6">
  <div class="section-label">BTS SIO</div>
  <h2>Épreuve E6</h2>
  <div class="projects-grid">
    <div class="project">
      <h3>Rsyslog</h3>
      <p>Centralisation et analyse des journaux systèmes.</p>
    </div>
    <div class="project">
      <h3>FOG</h3>
      <p>Déploiement automatisé d’images systèmes.</p>
    </div>
  </div>
</section>

<section id="contact">
  <div class="section-label">Contact</div>
  <h2>Me contacter</h2>
  <div class="card">
    📧 <a href="mailto:souleymanguendouz20@gmail.com">souleymanguendouz20@gmail.com</a><br><br>
    🔗 <a href="https://fr.linkedin.com/in/souleyman-guendouz-026957283" target="_blank">LinkedIn</a><br>
    💻 <a href="https://github.com/gdz933ecole" target="_blank">GitHub</a>
  </div>
</section>

<footer>
© 2025 — Guendouz Souleyman · BTS SIO SISR
</footer>

</body>
</html>
