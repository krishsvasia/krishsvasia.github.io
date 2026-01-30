---
layout: default
title: Projects
permalink: /projects/
---

<style>
  .project-grid {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
    justify-content: space-between;
    margin-top: 20px;
  }

  .project-card {
    background-color: #161b22; /* Dark card background */
    border: 1px solid #30363d; /* Subtle border */
    border-radius: 8px;
    padding: 24px;
    width: 48%; /* Two cards per row */
    box-sizing: border-box;
    transition: transform 0.2s, border-color 0.2s;
    margin-bottom: 20px;
    display: flex;
    flex-direction: column;
  }

  /* Hover Effect */
  .project-card:hover {
    transform: translateY(-3px);
    border-color: #58a6ff; /* Blue border on hover */
  }

  /* Typography inside cards */
  .project-card h3 {
    margin-top: 10px;
    margin-bottom: 10px;
    color: #58a6ff; /* Blue Title */
  }

  .project-card p {
    color: #8b949e; /* Grey text */
    font-size: 0.95em;
    flex-grow: 1; /* Pushes the link to the bottom */
  }

  /* Status Tags */
  .status-tag {
    display: inline-block;
    padding: 2px 10px;
    border-radius: 12px;
    font-size: 0.75em;
    font-weight: bold;
    text-transform: uppercase;
    width: fit-content;
  }
  
  .tag-wip { background: #d29922; color: #0d1117; }      /* Yellow/Gold */
  .tag-planned { background: #6e7681; color: #ffffff; }  /* Grey */
  .tag-done { background: #238636; color: #ffffff; }     /* Green */

  /* Mobile: Stack them 1 per row */
  @media (max-width: 768px) {
    .project-card { width: 100%; }
  }
</style>

<h2>🚀 Engineering Projects</h2>

<div class="project-grid">

  <div class="project-card">
    <span class="status-tag tag-wip"> In Progress</span>
    <h3>Zero-Copy Parser</h3>
    <p>A high-throughput C++20 library for parsing ITCH-style binary market data. Benchmarking <code>mmap</code> vs standard I/O.</p>
    <p><strong>Tech:</strong> C++, Linux API, Perf</p>
    <a href="#">View Code →</a>
  </div>

<div class="project-card">
    <span class="status-tag tag-done">✅ Completed</span>
    <h3>Adaptive Kalman Filter</h3>
    <p>A statistical arbitrage engine using a <strong>Vector Kalman Filter</strong> for multi-pair tracking.</p>
    <p><strong>Tech:</strong> Python, NumPy, Pandas, Monte Carlo</p>
    <a href="#">View Analytics Dashboard →</a>
  </div>
</div>

<hr style="border-color: #30363d; margin: 40px 0;">

<h2>🎓 Certifications</h2>

<div class="project-grid">
  
  <div class="project-card">
    <span class="status-tag tag-done">✅ Completed</span>
    <h3>Akuna Capital: Options 101</h3>
    <p>Deep dive into Options pricing models, The Greeks (Delta/Gamma), and Call/Put parity arbitrage.</p>
    <p><strong>Focus:</strong> Domain Knowledge</p>
  </div>

</div>
