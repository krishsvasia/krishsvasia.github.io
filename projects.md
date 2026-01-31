---
layout: default
title: Projects
permalink: /projects/
---

<style>
  .project-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 30px;
    margin-bottom: 40px;
  }

  .project-card {
    background-color: #21262d !important; 
    border: 1px solid #30363d;
    border-radius: 12px;
    padding: 25px;
    box-shadow: 0 4px 12px rgba(0,0,0,0.5);
    display: flex;
    flex-direction: column;
    height: 100%;
    transition: transform 0.2s;
  }

  .project-card:hover {
    transform: translateY(-5px);
    border-color: #58a6ff;
  }

  .project-card h3 {
    margin-top: 15px;
    font-size: 1.4rem;
    color: #ffffff !important;
  }

  .desc-text {
    font-size: 0.95rem;
    color: #8b949e;
    flex-grow: 1;
    margin-bottom: 20px;
    line-height: 1.5;
  }

  .tech-stack {
    font-size: 0.85rem;
    font-weight: bold;
    color: #c9d1d9;
    margin-bottom: 15px;
  }

  .status-tag {
    display: inline-block;
    padding: 4px 10px;
    border-radius: 20px;
    font-size: 0.75em;
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: 0.5px;
    margin-bottom: 10px;
  }
  
  .tag-wip { background: rgba(210, 153, 34, 0.15); color: #d29922; border: 1px solid #d29922; }
  .tag-planned { background: rgba(139, 148, 158, 0.15); color: #8b949e; border: 1px solid #8b949e; }
  .tag-done { background: rgba(46, 160, 67, 0.15); color: #3fb950; border: 1px solid #3fb950; }

  .card-link {
    display: block;
    text-align: center;
    background: #0d1117;
    color: #58a6ff !important;
    padding: 12px;
    border-radius: 6px;
    font-weight: bold;
    border: 1px solid #30363d;
    text-decoration: none !important;
  }
  .card-link:hover { background: #30363d; }

  @media (max-width: 900px) {
    .project-grid { grid-template-columns: 1fr; }
  }
</style>

<h2>Projects</h2>

<div class="project-grid">

  <div class="project-card">
      <div>
        <span class="status-tag tag-wip">In Progress</span>
        <h3>Adaptive Kalman Filter</h3>
        <p class="desc-text">Statistical arbitrage strategy using an adaptive noise algorithm for learning. Also includes circuit breaker logic and a transaction cost engine.</p>
        <p class="tech-stack">Python • Pandas • NumPy</p>
      </div>
      <a href="https://github.com/krishsvasia/kalman-filter-pairs-trading" class="card-link">View Code</a>
    </div>

</div>

<hr style="border-color: #30363d;">

<h2>Certifications</h2>

<div class="project-grid">
  
  <div class="project-card">
    <div>
      <span class="status-tag tag-done">Completed</span>
      <h3>Akuna Capital: Options 101</h3>
      <p class="desc-text">Deep dive into derivatives pricing, Call/Put Parity, and The Greeks (Delta/Gamma) for risk management logic.</p>
      <p class="tech-stack">Domain Knowledge • Finance</p>
    </div>
    <a href="#" class="card-link">View Certificate</a>
  </div>

</div>
