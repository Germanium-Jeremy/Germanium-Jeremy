<div align="center">

  <!-- Profile Header with Typewriter -->
  <h1>
    Hi there 👋, I'm <span style="color: #00d4ff;">NKUNDABAGENZI Jeremie</span>
  </h1>

  <div style="margin: 20px 0;">
    <img src="https://avatars.githubusercontent.com/u/151937776?v=4" width="180" height="180" style="border-radius: 50%; border: 5px solid #00d4ff; box-shadow: 0 0 30px rgba(0, 212, 255, 0.5);">
  </div>

  <!-- Typewriter Effect -->
  <div style="font-size: 1.4em; margin: 20px 0; min-height: 60px; font-family: monospace;">
    <span id="typewriter" style="color: #a5b4fc;"></span>
    <span class="cursor" style="color: #00d4ff;">|</span>
  </div>

  <p>
    <strong>Currently studying at Rwanda Coding Academy</strong><br>
    <em>Passionate about Software Engineering, AI & ML, Game Development and System Designs</em>
  </p>

  <a href="https://linkedin.com/in/nkundabagenzi-jeremie-3ba751405" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">
  </a>

  <hr style="border: 1px solid #334155; margin: 40px 0;">

  <!-- About Me -->
  <h2>🚀 About Me</h2>
  <p style="max-width: 700px; margin: 0 auto; font-size: 1.1em; line-height: 1.7;">
    I'm a 2026 computer science student with a strong passion for building elegant solutions to complex problems. When I'm not coding, you can find me exploring new technologies, contributing to open source, or personal hobby.
  </p>

  <br>

  <!-- Skills -->
  <h2>🛠️ Acquired Skills</h2>

  <div style="display: flex; flex-wrap: wrap; gap: 12px; justify-content: center; margin: 25px 0;">
    <!-- Replace these with your actual skills -->
    <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python">
    <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black" alt="JavaScript">
    <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript">
    <img src="https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB" alt="React">
    <img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=node.js&logoColor=white" alt="Node.js">
    <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker">
    <img src="https://img.shields.io/badge/AWS-FF9900?style=flat-square&logo=amazon-aws&logoColor=white" alt="AWS">
    <img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white" alt="Git">
  </div>

  <hr style="border: 1px solid #334155; margin: 40px 0;">

  <!-- Contact & Links -->
  <h2>📫 Let's Connect</h2>

  <p>
    <a href="mailto:nkundabagenzijeremy@gmail.com">
      <img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email">
    </a>
  </p>

  <br>

  <!-- Fun Stats / GitHub streak or trophies (optional) -->
  <h3>GitHub Stats</h3>
  <img src="https://github-readme-stats.vercel.app/api?username=Germanium-Jeremy&show_icons=true&theme=tokyonight&hide_border=true" alt="GitHub Stats">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=Germanium-Jeremy&theme=tokyonight&hide_border=true" alt="Streak Stats">

</div>

<script>
// Simple Typewriter Effect
const texts = [
  "Building the future, one commit at a time.",
  "Turning coffee into code ☕",
  "Student. Developer. Problem Solver.",
  "Always learning, always shipping."
];

let currentText = 0;
let charIndex = 0;
let isDeleting = false;
const typewriterElement = document.getElementById('typewriter');
const cursor = document.querySelector('.cursor');

function type() {
  const currentPhrase = texts[currentText];
  
  if (isDeleting) {
    typewriterElement.textContent = currentPhrase.substring(0, charIndex - 1);
    charIndex--;
  } else {
    typewriterElement.textContent = currentPhrase.substring(0, charIndex + 1);
    charIndex++;
  }

  let typeSpeed = 60;

  if (!isDeleting && charIndex === currentPhrase.length) {
    typeSpeed = 2000; // Pause at end of sentence
    isDeleting = true;
  } else if (isDeleting && charIndex === 0) {
    isDeleting = false;
    currentText = (currentText + 1) % texts.length;
    typeSpeed = 500;
  }

  setTimeout(type, typeSpeed);
}

// Start the typewriter
setTimeout(type, 1000);
</script>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;600&family=Space+Grotesk:wght@500;600&display=swap');
  
  body {
    font-family: 'Inter', system-ui, sans-serif;
  }
  
  h1, h2, h3 {
    font-family: 'Space Grotesk', sans-serif;
  }
  
  .cursor {
    animation: blink 0.7s step-end infinite;
  }
  
  @keyframes blink {
    50% { opacity: 0; }
  }
  
  /* Dark mode friendly colors */
  :root {
    --bg: #0f172a;
    --text: #e2e8f0;
  }
</style>
