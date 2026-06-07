<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Imaad Danish | NEXT LEVEL PORTFOLIO</title>

<style>

:root{
  --bg:#0a0f1f;
  --card:#111827;
  --card-hover:#1a2338;
  --primary:#4f8cff;
  --secondary:#7c3aed;
  --accent:#06b6d4;
  --text:#ffffff;
  --muted:#94a3b8;
  --border:rgba(255,255,255,.08);
}

*{
  margin:0;
  padding:0;
  box-sizing:border-box;
}

html{
  scroll-behavior:smooth;
}

body{
  font-family:Arial, Helvetica, sans-serif;
  background:var(--bg);
  color:var(--text);
  overflow-x:hidden;
}

/* NAVBAR */

nav{
  position:fixed;
  top:0;
  width:100%;
  display:flex;
  justify-content:space-between;
  align-items:center;
  padding:18px 7%;
  background:rgba(10,15,31,.95);
  backdrop-filter:blur(12px);
  border-bottom:1px solid var(--border);
  z-index:1000;
}

.logo{
  font-size:24px;
  font-weight:bold;
}

.logo span{
  color:var(--primary);
}

.nav-links{
  display:flex;
  gap:25px;
  list-style:none;
}

.nav-links a{
  color:white;
  text-decoration:none;
  transition:.3s;
}

.nav-links a:hover{
  color:var(--primary);
}

.menu-btn{
  display:none;
  font-size:28px;
  cursor:pointer;
}

/* HERO */

.hero{
  min-height:100vh;
  display:flex;
  justify-content:center;
  align-items:center;
  text-align:center;
  padding:120px 20px 80px;
}

.hero-content{
  max-width:900px;
}

.hero h1{
  font-size:clamp(3rem,8vw,6rem);
  margin-bottom:20px;
  line-height:1.1;
}

.hero h1 span{
  background:linear-gradient(
  90deg,
  var(--primary),
  var(--secondary),
  var(--accent));
  -webkit-background-clip:text;
  color:transparent;
}

.hero p{
  color:var(--muted);
  font-size:clamp(1rem,2vw,1.3rem);
  line-height:1.8;
}

.buttons{
  margin-top:35px;
  display:flex;
  justify-content:center;
  gap:15px;
  flex-wrap:wrap;
}

.btn{
  text-decoration:none;
  padding:14px 28px;
  border-radius:12px;
  font-weight:bold;
  transition:.3s;
}

.primary{
  background:linear-gradient(
  90deg,
  var(--primary),
  var(--secondary));
  color:white;
}

.secondary{
  border:1px solid var(--border);
  color:white;
}

.btn:hover{
  transform:translateY(-4px);
}

/* SECTION */

section{
  padding:90px 7%;
}

.title{
  text-align:center;
  font-size:clamp(2rem,5vw,3rem);
  margin-bottom:50px;
}

/* ABOUT */

.about{
  max-width:900px;
  margin:auto;
  text-align:center;
  color:var(--muted);
  line-height:1.9;
}

/* STATS */

.stats{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
  gap:20px;
  margin-top:50px;
}

.stat{
  background:var(--card);
  border:1px solid var(--border);
  padding:25px;
  border-radius:18px;
  text-align:center;
}

.stat h2{
  color:var(--primary);
  font-size:40px;
}

/* SKILLS */

.skills{
  display:flex;
  flex-wrap:wrap;
  justify-content:center;
  gap:15px;
}

.skills span{
  background:var(--card);
  border:1px solid var(--border);
  padding:12px 18px;
  border-radius:50px;
}

/* PROJECTS */

.projects{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(300px,1fr));
  gap:25px;
}

.card{
  background:var(--card);
  border:1px solid var(--border);
  border-radius:18px;
  padding:25px;
  transition:.3s;
}

.card:hover{
  transform:translateY(-8px);
  background:var(--card-hover);
}

.card p{
  color:var(--muted);
  margin-top:10px;
  line-height:1.7;
}

/* CONTACT */

.contact-form{
  max-width:700px;
  margin:auto;
  display:flex;
  flex-direction:column;
  gap:15px;
}

.contact-form input,
.contact-form textarea{
  background:var(--card);
  border:1px solid var(--border);
  border-radius:12px;
  padding:15px;
  color:white;
}

.contact-form textarea{
  min-height:180px;
}

.contact-form button{
  border:none;
  border-radius:12px;
  padding:15px;
  background:linear-gradient(
  90deg,
  var(--primary),
  var(--secondary));
  color:white;
  cursor:pointer;
}

.contact-grid{
  margin-top:25px;
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
  gap:20px;
}

.contact-card{
  background:var(--card);
  border:1px solid var(--border);
  border-radius:18px;
  padding:25px;
  text-align:center;
}

.contact-card a{
  color:var(--accent);
  text-decoration:none;
}

.whatsapp{
  display:inline-block;
  margin-top:25px;
  background:#25D366;
  color:white;
  text-decoration:none;
  padding:14px 24px;
  border-radius:12px;
}

/* FOOTER */

footer{
  text-align:center;
  padding:35px;
  border-top:1px solid var(--border);
  color:var(--muted);
}

/* EASTER LAB SYSTEM */

.easter-toggle {
  position: fixed;
  bottom: 30px;
  right: 30px;
  width: 45px;
  height: 45px;
  background: var(--primary);
  color: white;
  border: none;
  border-radius: 50%;
  font-weight: bold;
  cursor: pointer;
  z-index: 100;
  box-shadow: 0 4px 15px rgba(79, 140, 255, 0.3);
}

.easter-panel {
  position: fixed;
  top: 0;
  right: -400px;
  width: 400px;
  height: 100vh;
  background: #070d19;
  border-left: 1px solid var(--border);
  box-shadow: -10px 0 30px rgba(0,0,0,0.5);
  z-index: 1000;
  padding: 40px;
  transition: right 0.3s cubic-bezier(0.16, 1, 0.3, 1);
}

.easter-panel.open {
  right: 0;
}

.easter-panel h2 {
  margin-bottom: 10px;
}

.easter-panel p {
  color: var(--muted);
  font-size: 14px;
  line-height: 1.6;
}

.eyebrow {
  font-size: 12px;
  text-transform: uppercase;
  letter-spacing: 2px;
  color: var(--accent);
  font-weight: bold;
  margin-bottom: 5px;
}

.easter-close {
  position: absolute;
  top: 30px;
  right: 30px;
  background: transparent;
  border: none;
  color: var(--muted);
  font-size: 1.8rem;
  cursor: pointer;
}

.easter-embed-grid {
  display: flex;
  gap: 15px;
  margin-top: 30px;
}

/* MOBILE */

@media(max-width:768px){

  .menu-btn{
    display:block;
  }

  .nav-links{
    display:none;
    position:absolute;
    top:70px;
    left:0;
    width:100%;
    background:#0a0f1f;
    flex-direction:column;
    align-items:center;
    padding:20px;
  }

  .nav-links.active{
    display:flex;
  }

  .hero h1{
    font-size:42px;
  }

  .hero p{
    font-size:16px;
  }

  .buttons{
    flex-direction:column;
  }

  .btn{
    width:100%;
    text-align:center;
  }

  .projects{
    grid-template-columns:1fr;
  }

  .stats{
    grid-template-columns:1fr;
  }

  .contact-grid{
    grid-template-columns:1fr;
  }
}

</style>
</head>

<body>

<nav>
<div class="logo">
Imaad <span>Danish</span>
</div>

<div class="menu-btn" onclick="toggleMenu()">☰</div>

<ul class="nav-links" id="menu">
<li><a href="#about">About</a></li>
<li><a href="#skills">Skills</a></li>
<li><a href="#projects">Projects</a></li>
<li><a href="#contact">Contact</a></li>
</ul>
</nav>

<section class="hero">

<div class="hero-content">

<h1>Hello, I'm <span>Imaad Danish</span></h1>

<p>
Developer • AI Enthusiast • Robotics Explorer • Web Creator
Building innovative digital experiences through technology and creativity.
</p>

<div class="buttons">
<a href="#projects" class="btn primary">View Projects</a>
<a href="#contact" class="btn secondary">Contact Me</a>
</div>

</div>

</section>

<section id="about">

<h2 class="title">About Me</h2>

<p class="about">
I am passionate about Artificial Intelligence,
Robotics, Web Development and innovative technologies.
I enjoy creating projects that solve real-world problems
and continuously learning new skills.
</p>

<div class="stats">

<div class="stat">
<h2>15+</h2>
<p>Projects</p>
</div>

<div class="stat">
<h2>5+</h2>
<p>Technologies</p>
</div>

<div class="stat">
<h2>100%</h2>
<p>Passion</p>
</div>

<div class="stat">
<h2>24/7</h2>
<p>Learning</p>
</div>

</div>

</section>

<section id="skills">

<h2 class="title">Skills</h2>

<div class="skills">
<span>Python</span>
<span>HTML</span>
<span>CSS</span>
<span>JavaScript</span>
<span>Flutter</span>
<span>AI</span>
<span>Robotics</span>
<span>Web Development</span>
</div>

</section>

<section id="projects">

<h2 class="title">Projects</h2>

<div class="projects">

<div class="card">
<h3>AI Chatbot</h3>
<p>Smart conversational assistant powered by AI.</p>
</div>

<div class="card">
<h3>RobotX</h3>
<p>Robotics automation project with sensors.</p>
</div>

<div class="card">
<h3>Traffic Light System</h3>
<p>Smart traffic control simulation project.</p>
</div>

</div>

</section>

<section id="contact">

<h2 class="title">Contact Me</h2>

<form class="contact-form">
<input type="text" placeholder="Your Name" required>
<input type="email" placeholder="Your Email" required>
<textarea placeholder="Your Message"></textarea>
<button type="submit">Send Message</button>
</form>

<div class="contact-grid">

<div class="contact-card">
<h3>📧 Email</h3>
<br>
<a href="mailto:imaad.danish003@gmail.com">
imaad.danish003@gmail.com
</a>
</div>

<div class="contact-card">
<h3>📱 WhatsApp</h3>
<br>
<a href="https://wa.me/919997554431" target="_blank">
+91 99xxxxxxxx
</a>
</div>

</div>

<div style="text-align:center">
<a href="https://wa.me/919997554431" class="whatsapp" target="_blank">
💬 Chat on WhatsApp
</a>
</div>

</section>

<footer>
© 2026 Imaad Danish | NEXT LEVEL PORTFOLIO
       Developer●Robotics●Engineering
</footer>

<button
  class="easter-toggle"
  type="button"
  aria-label="Open hidden lab"
  data-easter-toggle
>
  67
</button>

<section class="easter-panel" aria-hidden="true" data-easter-panel>
  <button class="easter-close" type="button" aria-label="Close hidden lab" data-easter-close>
    ×
  </button>
  <p class="eyebrow">Hidden Lab</p>
  <h2>Technologia // 67</h2>
  <p>
    A tiny secret corner for the people who actually click around. Pure
    chaos, pure energy.
  </p>
  <div class="easter-embed-grid">
    <div class="easter-embed">
      <iframe
        width="110"
        height="200"
        src="https://www.myinstants.com/instant/67-sound-90775/embed/"
        frameborder="0"
        scrolling="no"
        title="67 soundboard"
      ></iframe>
    </div>
    <div class="easter-embed">
    <iframe
      width="110"
      height="200"
      src="https://www.myinstants.com/instant/technologia-53863/embed/"
      frameborder="0"
      scrolling="no"
      title="Technologia soundboard"
    ></iframe>
    </div>
  </div>
</section>

<script>
function toggleMenu(){
document.getElementById("menu").classList.toggle("active");
}

const toggleBtn = document.querySelector('[data-easter-toggle]');
const closeBtn = document.querySelector('[data-easter-close]');
const panel = document.querySelector('[data-easter-panel]');

if(toggleBtn && panel) {
  toggleBtn.addEventListener('click', () => {
    panel.classList.toggle('open');
    panel.setAttribute('aria-hidden', panel.classList.contains('open') ? 'false' : 'true');
  });
}
if(closeBtn && panel) {
  closeBtn.addEventListener('click', () => {
    panel.classList.remove('open');
    panel.setAttribute('aria-hidden', 'true');
  });
}
</script>
