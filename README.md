<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8"/>
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Indian Cyber Force // Cyber Ops Collective</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Roboto+Mono:wght@400;600;700&display=swap');

    body {
      font-family: 'Roboto Mono', monospace;
      background: radial-gradient(circle at center, #050510 0%, #020208 100%);
      color: #e2e8f0;
      overflow-x: hidden;
    }

    /* Particles background */
    #particles {
      position: fixed;
      top: 0; left: 0;
      width: 100%; height: 100%;
      z-index: -1;
      background: linear-gradient(120deg, #050510, #0a0d22);
    }

    /* Neon Title */
    .neon-title {
      font-weight: 700;
      text-transform: uppercase;
      font-size: clamp(2.5rem, 6vw, 5rem);
      background: linear-gradient(90deg, #00ffe5, #8b5cf6, #00ffe5);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      text-shadow: 0 0 20px rgba(0,255,229,0.3);
    }

    /* HUD cards */
    .hud-card {
      background: rgba(10, 15, 28, 0.5);
      border: 1px solid rgba(0,255,229,0.25);
      border-radius: 1rem;
      backdrop-filter: blur(16px);
      box-shadow: 0 0 25px rgba(0,255,229,0.15);
      transition: transform 0.3s, box-shadow 0.3s;
    }
    .hud-card:hover {
      transform: translateY(-5px) scale(1.01);
      box-shadow: 0 0 35px rgba(0,255,229,0.3);
    }

    /* Operation Feed */
    #feed {
      font-size: 0.9rem;
      color: #00ffe5;
      line-height: 1.4;
      min-height: 180px;
      white-space: pre-wrap;
    }

    /* Progress rings */
    .progress-ring {
      transform: rotate(-90deg);
    }
    .progress-text {
      transform: rotate(90deg);
    }

    /* System bars */
    .sys-bar {
      position: relative;
      width: 100%;
      height: 10px;
      background: rgba(255,255,255,0.05);
      border-radius: 9999px;
      overflow: hidden;
    }
    .sys-bar-fill {
      height: 100%;
      background: linear-gradient(90deg,#00ffe5,#8b5cf6);
      width: 0%;
      border-radius: 9999px;
      transition: width 2s ease-out;
    }

  </style>
</head>
<body class="p-6 sm:p-10">

  <!-- Background Particles -->
  <canvas id="particles"></canvas>

  <div class="max-w-6xl mx-auto space-y-12">

    <!-- Header -->
    <header class="text-center space-y-3">
      <h1 class="neon-title">INDIAN CYBER FORCE</h1>
      <p class="text-gray-400">Operating • From • Hidden • Binnary</p>
    </header>

    <!-- Operational Protocol -->
    <section class="hud-card p-6 sm:p-10 space-y-4">
      <h2 class="text-2xl font-bold text-cyan-300">OPERATIONAL PROTOCOL</h2>
      <p>
        We operate as a decentralized digital front, aligning with the doctrine of cyber sovereignty and national defense. <span class="text-cyan-400">digital resistance</span>.  
        We dont defend We hunt, We fuck their firwalls
        <span class="text-purple-400">Every operation leaves no trace — only resilience.</span>
      </p>
    </section>

    <section class="hud-card p-6 sm:p-10 space-y-6">
      <h2 class="text-2xl font-bold text-cyan-300">CORE ARCHIVE</h2>
      <div class="grid grid-cols-2 md:grid-cols-3 gap-6 justify-items-center">
        <div class="relative flex flex-col items-center">
          <svg class="progress-ring w-24 h-24">
            <circle cx="50%" cy="50%" r="40" stroke="#1f2937" stroke-width="8" fill="none"/>
            <circle class="ring" cx="50%" cy="50%" r="40" stroke="#00ffe5" stroke-width="8" fill="none" stroke-dasharray="251" stroke-dashoffset="251" stroke-linecap="round"/>
          </svg>
          <span class="absolute progress-text text-cyan-300 font-bold">85%</span>
          <p class="mt-2 text-sm">Cryptography</p>
        </div>
        <div class="relative flex flex-col items-center">
          <svg class="progress-ring w-24 h-24">
            <circle cx="50%" cy="50%" r="40" stroke="#1f2937" stroke-width="8" fill="none"/>
            <circle class="ring" cx="50%" cy="50%" r="40" stroke="#8b5cf6" stroke-width="8" fill="none" stroke-dasharray="251" stroke-dashoffset="251" stroke-linecap="round"/>
          </svg>
          <span class="absolute progress-text text-purple-400 font-bold">70%</span>
          <p class="mt-2 text-sm">Reverse Eng.</p>
        </div>
        <div class="relative flex flex-col items-center">
          <svg class="progress-ring w-24 h-24">
            <circle cx="50%" cy="50%" r="40" stroke="#1f2937" stroke-width="8" fill="none"/>
            <circle class="ring" cx="50%" cy="50%" r="40" stroke="#22c55e" stroke-width="8" fill="none" stroke-dasharray="251" stroke-dashoffset="251" stroke-linecap="round"/>
          </svg>
          <span class="absolute progress-text text-green-400 font-bold">52%</span>
          <p class="mt-2 text-sm">Kernel Ops</p>
        </div>
      </div>
    </section>

    <!-- New System Monitor Bars -->
    <section class="hud-card p-6 sm:p-10 space-y-6">
      <h2 class="text-2xl font-bold text-cyan-300">// SYSTEM METRICS</h2>
      <div class="space-y-4">
        <div>
          <p class="text-sm mb-1 text-gray-300">Network Integrity</p>
          <div class="sys-bar"><div class="sys-bar-fill" style="width:0%" data-width="95%"></div></div>
        </div>
        <div>
          <p class="text-sm mb-1 text-gray-300">Threat Detection</p>
          <div class="sys-bar"><div class="sys-bar-fill" style="width:0%" data-width="82%"></div></div>
        </div>
        <div>
          <p class="text-sm mb-1 text-gray-300">Uptime Stability</p>
          <div class="sys-bar"><div class="sys-bar-fill" style="width:0%" data-width="99%"></div></div>
        </div>
      </div>
    </section>

    <section class="hud-card p-6 sm:p-10 space-y-4">
      <h2 class="text-2xl font-bold text-cyan-300">// OPERATION FEED</h2>
      <div id="feed"></div>
    </section>

    <section class="hud-card p-6 sm:p-10 space-y-6">
      <h2 class="text-2xl font-bold text-cyan-300">// DATASTREAM ACTIVITY</h2>
      <div class="flex flex-wrap gap-6 justify-center">
        <img src="https://github-readme-stats.vercel.app/api?username=BharatCyberForce&show_icons=true&theme=tokyonight" class="rounded-lg"/>
        <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=BharatCyberForce&layout=compact&theme=tokyonight" class="rounded-lg"/>
      </div>
    </section>

    <!-- Encrypted Channels -->
    <section class="hud-card p-6 sm:p-10 space-y-4">
      <h2 class="text-2xl font-bold text-cyan-300">// ENCRYPTED CHANNELS</h2>
      <div class="flex gap-6 flex-wrap text-cyan-300">
        <a href="https://twitter.com/CyberForceX" class="hover:text-purple-400">Twitter</a>
        <a href="https://linkedin.com/in/IndianCyberForce" class="hover:text-purple-400">LinkedIn</a>
        <a href="mailto:BharatiyaCyberForce@protonmail.com" class="hover:text-purple-400">ProtonMail</a>
      </div>
    </section>

  </div>

  <!-- Particles Background -->
  <script>
    const canvas = document.getElementById('particles');
    const ctx = canvas.getContext('2d');
    canvas.width = window.innerWidth;
    canvas.height = window.innerHeight;
    let particles = [];
    for(let i=0; i<100; i++){
      particles.push({
        x: Math.random()*canvas.width,
        y: Math.random()*canvas.height,
        r: Math.random()*2+1,
        dx: (Math.random()-0.5)*0.5,
        dy: (Math.random()-0.5)*0.5
      });
    }
    function drawParticles(){
      ctx.clearRect(0,0,canvas.width,canvas.height);
      particles.forEach(p=>{
        ctx.beginPath();
        ctx.arc(p.x,p.y,p.r,0,Math.PI*2);
        ctx.fillStyle = "rgba(0,255,229,0.6)";
        ctx.fill();
        p.x+=p.dx; p.y+=p.dy;
        if(p.x<0||p.x>canvas.width) p.dx*=-1;
        if(p.y<0||p.y>canvas.height) p.dy*=-1;
      });
      requestAnimationFrame(drawParticles);
    }
    drawParticles();
  </script>

  <!-- Operation Feed Animation -->
  <script>
    const feed = document.getElementById('feed');
    const logs = [
      "[INIT] Secure grid node handshake established.",
      "[AUTH] Multi-factor cryptographic keys rotated.",
      "[TRACE] Zero-day reconnaissance executed.",
      "[DEFENSE] IDS anomaly signatures deployed.",
      "[MISSION] Operation Ghostline infiltration successful.",
      "[STATUS] Decentralized mesh integrity: GREEN."
    ];
    let i = 0;
    function addLog(){
      if(i<logs.length){
        feed.innerHTML += logs[i] + "\n";
        i++;
        setTimeout(addLog,1500);
      }
    }
    addLog();
  </script>

  <!-- Animate Rings + Bars -->
  <script>
    window.addEventListener("load", () => {
      const rings = document.querySelectorAll(".ring");
      const targetOffsets = [50, 80, 120]; // values that match your skills
      rings.forEach((ring, i) => {
        let current = 251;
        const target = targetOffsets[i];
        const interval = setInterval(() => {
          if(current <= target){ clearInterval(interval); }
          else {
            current -= 2;
            ring.setAttribute("stroke-dashoffset", current);
          }
        }, 15);
      });

      document.querySelectorAll(".sys-bar-fill").forEach(bar => {
        setTimeout(() => {
          bar.style.width = bar.dataset.width;
        }, 500);
      });
    });
  </script>

</body>
</html>
