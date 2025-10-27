<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>TrendHive - Internal Black Book</title>
<link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@700&display=swap" rel="stylesheet">
<style>
  * {margin:0; padding:0; box-sizing:border-box;}
  body {font-family:'Orbitron', sans-serif; background:#000; color:#f5f5f5; overflow-x:hidden;}
  a {color:#f5c842; text-decoration:none;}
  h1,h2,h3 {font-weight:700;}
  .container {width:90%; max-width:1200px; margin:0 auto; padding:50px 0;}
  .hero {position:relative; width:100%; height:100vh; display:flex; flex-direction:column; justify-content:center; align-items:center; text-align:center; background:url('https://i.imgur.com/your-hero-image.jpg') no-repeat center center/cover;}
  .hero h1 {font-size:5rem; color:#00bfff; text-shadow:2px 2px 15px rgba(0,0,0,0.7); margin-bottom:20px;}
  .hero p {font-size:2rem; color:#f5f5f5; text-shadow:1px 1px 10px rgba(0,0,0,0.6);}
  section {padding:80px 0; position:relative;}
  .section-title {font-size:3rem; color:#00bfff; margin-bottom:40px; text-align:center;}
  .cards {display:flex; flex-wrap:wrap; justify-content:center; gap:20px;}
  .card {background:rgba(20,20,20,0.85); border:1px solid #00bfff; border-radius:15px; padding:20px; width:250px; transition:0.3s; cursor:pointer;}
  .card:hover {transform:translateY(-10px); box-shadow:0 0 20px #00bfff;}
  .card img {width:100%; border-radius:10px; margin-bottom:15px;}
  .gallery {display:grid; grid-template-columns:repeat(auto-fit, minmax(250px,1fr)); gap:15px;}
  .gallery img {width:100%; border-radius:10px; transition:0.3s; cursor:pointer;}
  .gallery img:hover {transform:scale(1.05); box-shadow:0 0 15px #00bfff;}
  .buzzword {position:absolute; color:#00bfff; font-weight:bold; opacity:0.8; animation:floatUp 5s ease-out infinite;}
  @keyframes floatUp {0%{transform:translateY(0); opacity:0.8;}100%{transform:translateY(-80px); opacity:0;}}
  .footer {text-align:center; padding:50px 0; font-size:0.9rem; color:#888;}
</style>
</head>
<body>

<!-- Hero -->
<div class="hero">
  <h1>TrendHive</h1>
  <p>Attention Organized</p>
</div>

<!-- Mission -->
<section>
  <div class="container">
    <h2 class="section-title">Mission</h2>
    <p style="text-align:center; font-size:1.5rem; max-width:800px; margin:0 auto;">
      TrendHive organizes attention in the digital world, surfacing meaningful insights before trends emerge. Unlike traditional social platforms, we focus on curated engagement, actionable insights, and predictive intelligence—giving users and investors the edge in real time.
    </p>
  </div>
</section>

<!-- Tech Stack / Architecture -->
<section style="background:rgba(0,0,0,0.9);">
  <div class="container">
    <h2 class="section-title">Tech Stack & Architecture</h2>
    <div class="cards">
      <div class="card">
        <h3>Frontend</h3>
        <p>React, TailwindCSS, Mobile-Optimized UI</p>
      </div>
      <div class="card">
        <h3>Backend</h3>
        <p>Node.js, Express, Python Microservices</p>
      </div>
      <div class="card">
        <h3>Data</h3>
        <p>BigQuery, PostgreSQL, Real-time Simulations</p>
      </div>
      <div class="card">
        <h3>AI & ML</h3>
        <p>Trend Prediction, Attention Analysis, Pattern Recognition</p>
      </div>
    </div>
  </div>
</section>

<!-- Differentiation & Defensibility -->
<section>
  <div class="container">
    <h2 class="section-title">Differentiation & Defensibility</h2>
    <p style="text-align:center; font-size:1.3rem; max-width:900px; margin:0 auto;">
      TrendHive leverages proprietary AI algorithms and real-time predictive modeling to identify trends before they go viral. Unlike existing social platforms, our defensibility lies in our data aggregation model, predictive insights, and high-quality attention curation that competitors cannot replicate at scale.
    </p>
  </div>
</section>

<!-- Founder -->
<section style="background:rgba(0,0,0,0.9);">
  <div class="container">
    <h2 class="section-title">Founder</h2>
    <div class="cards">
      <div class="card">
        <h3>Your Name</h3>
        <p>Founder & CEO</p>
        <p>Unique positioning to execute on the next generation of social attention, blending tech expertise, vision, and market timing.</p>
      </div>
    </div>
  </div>
</section>

<!-- Image Gallery -->
<section>
  <div class="container">
    <h2 class="section-title">Concept Visuals</h2>
    <div class="gallery">
      <img src="https://i.imgur.com/1.jpg" alt="Visual 1">
      <img src="https://i.imgur.com/2.jpg" alt="Visual 2">
      <img src="https://i.imgur.com/3.jpg" alt="Visual 3">
      <img src="https://i.imgur.com/4.jpg" alt="Visual 4">
    </div>
  </div>
</section>

<!-- Footer -->
<div class="footer">
  TrendHive Internal Presentation • All rights reserved
</div>

<!-- Simulated Floating Buzzwords -->
<script>
  const buzzwords = ['AI','Tech','Buzz','Hot','Engagement','Metrics','Growth','Attention','Prediction'];
  function spawnBuzzwords(){
    for(let i=0;i<5;i++){
      const div = document.createElement('div');
      div.className='buzzword';
      div.textContent=buzzwords[Math.floor(Math.random()*buzzwords.length)];
      div.style.left=Math.random()*window.innerWidth+'px';
      div.style.top=Math.random()*window.innerHeight+'px';
      div.style.fontSize=(14+Math.random()*24)+'px';
      document.body.appendChild(div);
      setTimeout(()=>div.remove(),5000+Math.random()*3000);
    }
  }
  setInterval(spawnBuzzwords,700);
</script>

<script>
// Define the formulas as strings
const formulas = [
  "A_s = (Interactions*w_i + Shares*w_s + Comments*w_c)/TimeDecay",
  "V_t = (A_s(t) - A_s(t-Δt))/Δt",
  "SNR = Signal/(Noise+1)",
  "C_p = Σ(α_i * A_s_i)",
  "E_n = A_s / Followers^β",
  "A_s_adjusted = A_s * e^(-λ*t)",
  "T_c = γ1*V_t + γ2*SNR + γ3*C_p",
  "Similarity = |A ∩ B| / |A ∪ B|"
];

function spawnFormula() {
  const formula = formulas[Math.floor(Math.random()*formulas.length)];
  const el = document.createElement('div');
  el.className = 'floating-formula';
  el.textContent = formula;
  el.style.left = Math.random()*80 + 'vw';
  el.style.top = Math.random()*80 + 'vh';
  document.getElementById('dashboard').appendChild(el);
  setTimeout(() => el.remove(), 4000);
}

// Call periodically to spawn formulas randomly
setInterval(spawnFormula, 1500);
</script>

.floating-formula {
  position: absolute;
  font-family: 'Courier New', monospace;
  font-size: 14px;
  color: #00ff00;
  opacity: 0.8;
  animation: floatUp 4s ease-out forwards;
  text-shadow: 0 0 5px #00ff00;
}

@keyframes floatUp {
  0% {transform: translateY(0); opacity:0.8;}
  100% {transform: translateY(-60px); opacity:0;}
}
</style>

</script>
</body>
</html>
