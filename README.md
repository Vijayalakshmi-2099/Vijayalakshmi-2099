```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Vijayalakshmi | Developer Portfolio</title>

<style>
*{margin:0;padding:0;box-sizing:border-box;scroll-behavior:smooth}
:root{--bg:#080b16;--card:#11182b;--text:#f4f6ff;--muted:#a8b1ca;--blue:#6c63ff;--cyan:#37e6ff}
body{font-family:Arial,sans-serif;background:var(--bg);color:var(--text);overflow-x:hidden}
a{text-decoration:none;color:inherit}
nav{position:fixed;top:0;width:100%;padding:18px 8%;display:flex;justify-content:space-between;align-items:center;background:#080b16df;backdrop-filter:blur(15px);z-index:100;border-bottom:1px solid #ffffff12}
.logo{font-size:23px;font-weight:bold;color:var(--cyan)}
nav ul{display:flex;gap:25px;list-style:none}
nav a:hover{color:var(--cyan)}
section{padding:100px 9%;scroll-margin-top:65px}
.hero{min-height:100vh;display:flex;align-items:center;justify-content:space-between;gap:40px;background:radial-gradient(ellipse at 80% 40%,#39308045,transparent 50%)}
.hero-content{max-width:700px}
.tag{color:var(--cyan);letter-spacing:3px;font-size:13px;text-transform:uppercase}
h1{font-size:clamp(38px,6vw,70px);line-height:1.15;margin:20px 0}
.gradient{background:linear-gradient(90deg,var(--cyan),#9d85ff,var(--blue));background-clip:text;-webkit-background-clip:text;color:transparent}
.hero p,.about p{font-size:17px;line-height:1.9;color:var(--muted)}
.buttons{display:flex;gap:15px;flex-wrap:wrap;margin-top:30px}
.btn{padding:13px 22px;border-radius:10px;background:linear-gradient(120deg,var(--blue),#8b5cf6);font-weight:bold;transition:.3s;display:inline-block}
.btn:hover{transform:translateY(-4px);box-shadow:0 10px 30px #6c63ff55}
.btn.outline{background:transparent;border:1px solid var(--cyan)}
.avatar{width:260px;height:260px;flex-shrink:0;border-radius:50%;display:grid;place-items:center;font-size:100px;background:linear-gradient(135deg,#6c63ff,#37e6ff);box-shadow:0 0 70px #6c63ff55;animation:float 4s ease-in-out infinite}
@keyframes float{0%,100%{transform:translateY(0)}50%{transform:translateY(-18px)}}
.heading{text-align:center;font-size:36px;margin-bottom:15px}
.subtitle{text-align:center;color:var(--muted);margin-bottom:45px}
.about,.skill-card,.project,.edu-card,.contact-box{background:var(--card);border:1px solid #ffffff12;border-radius:18px;padding:28px;transition:.35s}
.about:hover,.skill-card:hover,.project:hover,.edu-card:hover{transform:translateY(-7px);border-color:var(--blue);box-shadow:0 15px 40px #0004}
.stats{display:grid;grid-template-columns:repeat(3,1fr);gap:15px;margin-top:25px}
.stat{text-align:center;padding:20px;background:#ffffff06;border-radius:12px}
.stat strong{display:block;color:var(--cyan);font-size:26px;margin-bottom:8px}
.stat span{font-size:13px;color:var(--muted)}
.grid{display:grid;grid-template-columns:repeat(3,1fr);gap:22px}
.skill-card h3,.project h3,.edu-card h3{margin-bottom:15px}
.skill-card p,.project p,.edu-card p{color:var(--muted);line-height:1.8}
.icon{font-size:30px;margin-bottom:15px}
.chips{display:flex;flex-wrap:wrap;gap:8px;margin-top:18px}
.chip{font-size:12px;padding:7px 11px;background:#6c63ff20;color:#bcb8ff;border-radius:20px}
.project{display:flex;flex-direction:column}
.project .btn{align-self:flex-start;margin-top:22px}
.project p{flex-grow:1}
.project .project-label{color:var(--cyan);font-size:12px;margin-bottom:10px}
.timeline{max-width:800px;margin:auto;display:grid;gap:20px}
.edu-card{border-left:3px solid var(--blue)}
.edu-card small{display:block;color:var(--cyan);margin-bottom:10px}
.contact-box{text-align:center;max-width:750px;margin:auto}
.contact-box p{color:var(--muted);line-height:1.8;margin:15px 0 25px}
.contact-links{display:flex;justify-content:center;gap:15px;flex-wrap:wrap}
footer{text-align:center;padding:28px;color:var(--muted);border-top:1px solid #ffffff12}
.reveal{opacity:0;transform:translateY(35px);transition:opacity .8s ease,transform .8s ease}
.reveal.show{opacity:1;transform:translateY(0)}
.cursor{display:inline-block;color:var(--cyan);animation:blink .7s infinite}
@keyframes blink{50%{opacity:0}}
#topBtn{position:fixed;bottom:25px;right:25px;border:none;border-radius:50%;width:45px;height:45px;background:var(--blue);color:white;font-size:22px;cursor:pointer;display:none;z-index:99}
@media(max-width:900px){.grid{grid-template-columns:repeat(2,1fr)}.avatar{width:190px;height:190px;font-size:75px}}
@media(max-width:650px){nav{padding:16px 5%}nav ul{gap:12px;font-size:12px}.hero{flex-direction:column-reverse;justify-content:center;text-align:center;padding-top:130px}.avatar{width:150px;height:150px;font-size:60px}.buttons{justify-content:center}.grid{grid-template-columns:1fr}.stats{grid-template-columns:1fr}.heading{font-size:30px}section{padding:80px 6%}}
</style>
</head>
<body>

<nav>
  <a href="#home" class="logo">VJ.</a>
  <ul>
    <li><a href="#home">Home</a></li>
    <li><a href="#about">About</a></li>
    <li><a href="#skills">Skills</a></li>
    <li><a href="#projects">Projects</a></li>
    <li><a href="#contact">Contact</a></li>
  </ul>
</nav>

<section class="hero" id="home">
  <div class="hero-content">
    <span class="tag">Welcome to my portfolio</span>
    <h1>Hi, I'm <span class="gradient">Vijayalakshmi</span></h1>
    <h2 style="font-size:clamp(22px,3vw,34px);margin-bottom:20px">
      I'm a <span class="gradient" id="typing"></span><span class="cursor">|</span>
    </h2>
    <p>I'm a Computer Science and Engineering student specializing in AI & ML, passionate about Python development, problem-solving, and building useful software applications.</p>
    <div class="buttons">
      <a class="btn" href="#projects">Explore My Projects ↗</a>
      <a class="btn outline" href="#contact">Contact Me</a>
    </div>
  </div>
  <div class="avatar">👩🏻‍💻</div>
</section>

<section id="about">
  <h2 class="heading reveal">About <span class="gradient">Me</span></h2>
  <p class="subtitle reveal">A little introduction about myself</p>
  <div class="about reveal">
    <p>I'm pursuing a B.Tech in Computer Science and Engineering (AI & ML) at Tirumala Engineering College. I enjoy learning programming, developing projects, and improving my technical skills through hands-on practice.</p>
    <p style="margin-top:15px">My technical interests include Python programming, SQL databases, backend development, and machine learning. I aim to contribute to meaningful software projects while continuously learning new technologies.</p>
    <div class="stats">
      <div class="stat"><strong>8.31</strong><span>B.Tech CGPA (as listed)</span></div>
      <div class="stat"><strong>3</strong><span>Core skills: C, Python, SQL</span></div>
      <div class="stat"><strong>2027</strong><span>Expected graduation</span></div>
    </div>
  </div>
</section>

<section id="skills">
  <h2 class="heading reveal">Technical <span class="gradient">Skills</span></h2>
  <p class="subtitle reveal">Technologies and tools I work with</p>
  <div class="grid">
    <div class="skill-card reveal">
      <div class="icon">💻</div><h3>Programming</h3>
      <p>Building programming fundamentals and solving logical problems.</p>
      <div class="chips"><span class="chip">Python</span><span class="chip">C</span></div>
    </div>
    <div class="skill-card reveal">
      <div class="icon">🗄️</div><h3>Database</h3>
      <p>Working with structured data and learning database queries.</p>
      <div class="chips"><span class="chip">SQL</span><span class="chip">MySQL</span></div>
    </div>
    <div class="skill-card reveal">
      <div class="icon">🛠️</div><h3>Developer Tools</h3>
      <p>Tools used for coding, experimentation, and project development.</p>
      <div class="chips"><span class="chip">VS Code</span><span class="chip">Google Colab</span><span class="chip">GitHub</span></div>
    </div>
    <div class="skill-card reveal">
      <div class="icon">🌐</div><h3>Backend Development</h3>
      <p>Experience building a Flask API for house price predictions.</p>
      <div class="chips"><span class="chip">Python</span><span class="chip">Flask API</span></div>
    </div>
    <div class="skill-card reveal">
      <div class="icon">🤖</div><h3>AI & Machine Learning</h3>
      <p>Academic specialization with practical project exposure to model training.</p>
      <div class="chips"><span class="chip">AI & ML</span><span class="chip">Data preprocessing</span></div>
    </div>
    <div class="skill-card reveal">
      <div class="icon">🤝</div><h3>Soft Skills</h3>
      <p>Adaptability, teamwork, willingness to learn, and a supportive attitude.</p>
      <div class="chips"><span class="chip">Teamwork</span><span class="chip">Learning</span></div>
    </div>
  </div>
</section>

<section id="projects">
  <h2 class="heading reveal">My <span class="gradient">Projects</span></h2>
  <p class="subtitle reveal">Projects that reflect my learning and development</p>
  <div class="grid">
    <article class="project reveal">
      <div class="icon">🎯</div>
      <span class="project-label">PROJECT 01 · C PROGRAMMING</span>
      <h3>Number Guessing Game</h3>
      <p>A simple interactive game in which the computer generates a random number and the player tries to guess it. The program provides feedback when a guess is too high, too low, or correct.</p>
      <div class="chips"><span class="chip">C</span><span class="chip">Loops</span><span class="chip">Conditionals</span></div>
      <a class="btn" href="https://github.com/Vijayalakshmi-2931" target="_blank" rel="noopener">View GitHub ↗</a>
    </article>
    <article class="project reveal">
      <div class="icon">🏠</div>
      <span class="project-label">PROJECT 02 · PYTHON / ML</span>
      <h3>House Price Prediction</h3>
      <p>A machine learning project focused on data preprocessing and model training to predict house prices. A Flask API was developed to provide predictions through application requests.</p>
      <div class="chips"><span class="chip">Python</span><span class="chip">Machine Learning</span><span class="chip">Flask API</span></div>
      <a class="btn" href="https://github.com/Vijayalakshmi-2931" target="_blank" rel="noopener">View GitHub ↗</a>
    </article>
    <article class="project reveal">
      <div class="icon">📚</div>
      <span class="project-label">CONTINUOUS LEARNING</span>
      <h3>Python & SQL Practice</h3>
      <p>Practicing programming fundamentals, logical problem-solving, database queries, and software development concepts to strengthen my technical foundation.</p>
      <div class="chips"><span class="chip">Python</span><span class="chip">SQL</span><span class="chip">Problem-solving</span></div>
      <a class="btn" href="https://github.com/Vijayalakshmi-2931" target="_blank" rel="noopener">Visit GitHub ↗</a>
    </article>
  </div>
</section>

<section id="education">
  <h2 class="heading reveal">Education & <span class="gradient">Experience</span></h2>
  <p class="subtitle reveal">My academic background and internship</p>
  <div class="timeline">
    <div class="edu-card reveal">
      <small>2023 – 2027</small>
      <h3>B.Tech – Computer Science & Engineering (AI & ML)</h3>
      <p>Tirumala Engineering College, Jonnalagadda, Narasaraopet</p>
      <p>CGPA: 8.31</p>
    </div>
    <div class="edu-card reveal">
      <small>2022 – 2023</small>
      <h3>Intermediate – MPC</h3>
      <p>Sri Sadhana Junior College, Markapur</p>
      <p>Percentage: 75.2%</p>
    </div>
    <div class="edu-card reveal">
      <small>2020 – 2021</small>
      <h3>SSC</h3>
      <p>Z.P. High School (Girls), Markapur</p>
      <p>Percentage: 98%</p>
    </div>
    <div class="edu-card reveal">
      <small>April 2026 – June 2026</small>
      <h3>Python Intern – Vaults of Codes</h3>
      <p>Completed a virtual internship involving Python programming, problem-solving, software development, debugging, and application development under mentor guidance.</p>
    </div>
  </div>
</section>

<section id="certifications">
  <h2 class="heading reveal">Certifications & <span class="gradient">Languages</span></h2>
  <p class="subtitle reveal">My learning journey</p>
  <div class="grid">
    <div class="skill-card reveal"><div class="icon">📜</div><h3>Introduction to C Programming</h3><p>Programming fundamentals and basic problem-solving.</p></div>
    <div class="skill-card reveal"><div class="icon">🐍</div><h3>Core Python</h3><p>Python fundamentals and programming concepts.</p></div>
    <div class="skill-card reveal"><div class="icon">🗃️</div><h3>SQL – IBM Skills Network</h3><p>Database concepts and SQL query fundamentals.</p></div>
  </div>
  <div class="buttons" style="justify-content:center;margin-top:25px">
    <span class="chip">English</span><span class="chip">Telugu</span>
  </div>
</section>

<section id="contact">
  <h2 class="heading reveal">Let's <span class="gradient">Connect</span></h2>
  <p class="subtitle reveal">I'm open to entry-level opportunities and learning experiences</p>
  <div class="contact-box reveal">
    <div class="icon">💌</div>
    <h3>Have an opportunity in mind?</h3>
    <p>Feel free to connect with me for software development opportunities, collaborations, or professional discussions.</p>
    <div class="contact-links">
      <a class="btn" href="mailto:vijayalakshmikukatlapalli427@gmail.com">Email Me ↗</a>
      <a class="btn outline" href="https://github.com/Vijayalakshmi-2931" target="_blank" rel="noopener">GitHub ↗</a>
      <a class="btn outline" href="https://www.linkedin.com/" target="_blank" rel="noopener">LinkedIn ↗</a>
    </div>
  </div>
</section>

<footer>
  <p>Designed with 💜 by Vijayalakshmi</p>
  <p style="margin-top:10px;font-size:12px">© <span id="year"></span> Vijayalakshmi. All rights reserved.</p>
</footer>

<button id="topBtn" aria-label="Back to top" title="Back to top">↑</button>

<script>
const words=["Python Developer","Software Developer","AI & ML Student","Problem Solver"];
let wordIndex=0,charIndex=0,deleting=false;
const typing=document.getElementById("typing");

function typeEffect(){
  const word=words[wordIndex];
  typing.textContent=word.substring(0,charIndex);
  if(!deleting){
    charIndex++;
    if(charIndex>word.length){
      deleting=true;
      setTimeout(typeEffect,1100);
      return;
    }
  }else{
    charIndex--;
    if(charIndex<0){
      charIndex=0;
      deleting=false;
      wordIndex=(wordIndex+1)%words.length;
    }
  }
  setTimeout(typeEffect,deleting?45:90);
}
typeEffect();

const observer=new IntersectionObserver(entries=>{
  entries.forEach(entry=>{
    if(entry.isIntersecting){
      entry.target.classList.add("show");
      observer.unobserve(entry.target);
    }
  });
},{threshold:0.12});

document.querySelectorAll(".reveal").forEach(el=>observer.observe(el));

const topBtn=document.getElementById("topBtn");
window.addEventListener("scroll",()=>{
  topBtn.style.display=window.scrollY>400?"block":"none";
});
topBtn.addEventListener("click",()=>{
  window.scrollTo({top:0,behavior:"smooth"});
});

document.getElementById("year").textContent=new Date().getFullYear();
</script>
</body>
</html>
```
