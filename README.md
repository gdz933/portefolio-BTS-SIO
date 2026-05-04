<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <title>Guendouz Souleyman — Portfolio</title>
  <meta name="description" content="Portfolio de Guendouz Souleyman, étudiant BTS SIO SISR spécialisé systèmes, réseaux et cybersécurité.">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@400;500;700&family=JetBrains+Mono:wght@400;600&display=swap" rel="stylesheet">

  <style>
    :root {
      --blue:#00aaff;
      --bg:#0d0d0f;
      --bg2:#141418;
      --text:#f0f0f0;
      --muted:#888;
      --border:rgba(255,255,255,.07);
    }

    *{margin:0;padding:0;box-sizing:border-box}
    html{scroll-behavior:smooth}
    body{
      font-family:'Space Grotesk',sans-serif;
      background:var(--bg);
      color:var(--text);
      line-height:1.6;
    }

    /* NAV */
    nav{
      position:fixed;
      top:0;left:0;right:0;
      height:60px;
      display:flex;
      align-items:center;
      justify-content:space-between;
      padding:0 32px;
      background:rgba(13,13,15,.85);
      backdrop-filter:blur(12px);
      border-bottom:1px solid var(--border);
      z-index:100;
      transition:box-shadow .3s;
    }
    nav .logo{
      font-family:'JetBrains Mono',monospace;
      color:var(--blue);
      font-size:.85em;
    }
    nav ul{
      display:flex;
      list-style:none;
      gap:28px;
    }
    nav a{
      color:var(--muted);
      text-decoration:none;
      font-size:.9em;
    }
    nav a:hover{color:var(--text)}

    .burger{
      display:none;
      font-size:1.6em;
      cursor:pointer;
    }

    /* HERO */
    header{
      min-height:100vh;
      display:flex;
      flex-direction:column;
      justify-content:center;
      align-items:center;
      text-align:center;
      padding:100px 20px 60px;
      position:relative;
    }
    header::before{
      content:"";
      position:absolute;
      inset:0;
      background:url("https://www.fond-ecran-hd.net/Public/uploads/2019-01-14/thumbs-1/1397.jpg") center/cover;
      opacity:.12;
    }
    header>*{position:relative}

    .badge{
      font-family:'JetBrains Mono';
      font-size:.75em;
      color:var(--blue);
      border:1px solid rgba(0,170,255,.3);
      padding:6px 14px;
      border-radius:20px;
      margin-bottom:20px;
    }
    header h1{
      font-size:clamp(2.3em,6vw,4em);
      line-height:1.1;
    }
    header h1 span{color:var(--blue)}
    .subtitle{
      max-width:500px;
      color:var(--muted);
      margin:20px auto 36px;
    }

    .button{
      padding:12px 26px;
      border-radius:8px;
      font-size:.9em;
      text-decoration:none;
      transition:.25s;
      display:inline-block;
    }
    .primary{background:var(--blue);color:#000}
    .primary:hover{transform:translateY(-2px)}
    .outline{
      border:1px solid var(--border);
      color:var(--text);
    }

    section{
      max-width:960px;
      margin:auto;
      padding:80px 24px;
    }
    h2{margin-bottom:36px}

    /* SKILLS */
    .skills-grid{
      display:grid;
      grid-template-columns:repeat(auto-fill,minmax(200px,1fr));
      gap:14px;
    }
    .skill{
      background:var(--bg2);
      padding:18px;
      border-radius:10px;
      border:1px solid var(--border);
    }
    .bar-bg{
      height:5px;
      background:rgba(255,255,255,.1);
      border-radius:5px;
      overflow:hidden;
      margin-top:10px;
    }
    .bar{
      height:100%;
      width:0;
      background:linear-gradient(90deg,var(--blue),#66ccff);
      transition:width 1s ease;
    }

    /* PROJECTS */
    .project{
      background:var(--bg2);
      border:1px solid var(--border);
      padding:26px;
      border-radius:12px;
      margin-bottom:20px;
      transition:.3s;
    }
    .project:hover{
      transform:translateY(-4px);
      box-shadow:0 10px 30px rgba(0,170,255,.15);
    }

    /* CONTACT */
    .contact-grid{
      display:grid;
      grid-template-columns:1fr 1fr;
      gap:40px;
    }
    input,textarea{
      width:100%;
      background:var(--bg2);
      border:1px solid var(--border);
      color:var(--text);
      padding:12px;
      border-radius:8px;
    }

    footer{
      text-align:center;
      padding:30px;
      border-top:1px solid var(--border);
      font-family:'JetBrains Mono';
      color:var(--muted);
    }

    /* MOBILE */
    @media(max-width:700px){
      nav ul{
        position:absolute;
        top:60px;
        right:20px;
        background:var(--bg2);
        flex-direction:column;
        padding:20px;
        border-radius:10px;
        display:none;
      }
      nav ul.active{display:flex}
      .burger{display:block}
      .contact-grid{grid-template-columns:1fr}
    }
  </style>
</head>

<body>

<nav>
  <span class="logo">GS.dev</span>
  <div class="burger">☰</div>
  <ul>
    <li><a href="#skills">Compétences</a></li>
    <li><a href="#projects">Projets</a></li>
    <li><a href="#contact">Contact</a></li>
  </ul>
</nav>

<header>
  <div class="badge">BTS SIO · SISR</div>
  <h1>Guendouz<br><span>Souleyman</span></h1>
  <p class="subtitle">Étudiant passionné par les systèmes, réseaux et la cybersécurité.</p>
  <a href="#projects" class="button primary">Voir mes projets</a>
</header>

<section id="skills">
  <h2>Compétences</h2>
  <div class="skills-grid">
    <div class="skill">Windows Server<div class="bar-bg"><div class="bar" data-width="80%"></div></div></div>
    <div class="skill">Active Directory<div class="bar-bg"><div class="bar" data-width="75%"></div></div></div>
    <div class="skill">Linux<div class="bar-bg"><div class="bar" data-width="65%"></div></div></div>
    <div class="skill">Réseaux TCP/IP<div class="bar-bg"><div class="bar" data-width="70%"></div></div></div>
  </div>
</section>

<section id="projects">
  <h2>Projets</h2>
  <div class="project">
    <h3>Serveur Windows AD</h3>
    <p>Mise en place Active Directory, DNS, DHCP sous VMware.</p>
  </div>
  <div class="project">
    <h3>Portfolio Web</h3>
    <p>Site responsive HTML / CSS dark mode.</p>
  </div>
</section>

<section id="contact">
  <h2>Contact</h2>
  <div class="contact-grid">
    <div>
      <p>Email : <strong>souleymanghuendouz20@gmail.com</strong></p>
      <p>GitHub / LinkedIn à ajouter</p>
    </div>
    <form>
      <input placeholder="Nom"><br><br>
      <input placeholder="Email"><br><br>
      <textarea placeholder="Message"></textarea><br><br>
      <button class="button primary">Envoyer</button>
    </form>
  </div>
</section>

<footer>
  © 2025 — Guendouz Souleyman
</footer>

<script>
/* menu mobile */
const burger=document.querySelector(".burger");
const menu=document.querySelector("nav ul");
burger.onclick=()=>menu.classList.toggle("active");

/* navbar scroll */
window.addEventListener("scroll",()=>{
  document.querySelector("nav").style.boxShadow=
    window.scrollY>20?"0 5px 20px rgba(0,0,0,.4)":"none";
});

/* skills animation */
const bars=document.querySelectorAll(".bar");
const obs=new IntersectionObserver(entries=>{
  entries.forEach(e=>{
    if(e.isIntersecting){
      e.target.style.width=e.target.dataset.width;
    }
  });
},{threshold:.5});
bars.forEach(b=>obs.observe(b));
</script>

</body>
</html>
