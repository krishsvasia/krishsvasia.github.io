---
layout: default
title: Projects
permalink: /projects/
---

<style>
/* 1. The Container: Force 3 Columns */
  .project-grid {
    display: grid;
    /* This creates exactly 3 equal columns */
    grid-template-columns: repeat(3, 1fr); 
    gap: 20px; /* Space between cards */
    margin-bottom: 40px;
  }

  /* 2. The Cards: Reset width */
  .project-card {
    background: #ffffff; /* Use #161b22 for Dark Mode */
    border: 1px solid #e1e4e8;
    border-radius: 6px;
    padding: 20px;
    /* Do NOT set width here, the Grid handles it */
    width: auto; 
    box-sizing: border-box;
    transition: transform 0.2s;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
  }

  /* 3. Mobile Protection: Stack them on phones */
  @media (max-width: 900px) {
    .project-grid {
      /* On tablets/phones, switch to 1 column so they don't get squished */
      grid-template-columns: 1fr; 
    }
  }</style>

<h2>Engineering Projects</h2>

<div class="project-grid">

  <div class="project-card">
    <span class="status-tag tag-wip"> In Progress</span>
    <h3>Zero-Copy Parser</h3>
    <p>A high-throughput C++20 library for parsing ITCH-style binary market data. Benchmarking <code>mmap</code> vs standard I/O.</p>
    <p><strong>Tech:</strong> C++, Linux API, Perf</p>
    <a href="#">View Code →</a>
  </div>

<div class="project-card">
    <span class="status-tag tag-done">Completed</span>
    <h3>Adaptive Kalman Filter</h3>
    <p>A statistical arbitrage engine using a <strong>Vector Kalman Filter</strong> for multi-pair tracking.</p>
    <p><strong>Tech:</strong> Python, NumPy, Pandas, Monte Carlo</p>
    <a href="#">View Analytics Dashboard →</a>
  </div>
</div>

<hr style="border-color: #30363d; margin: 40px 0;">

<h2>Certifications</h2>

<div class="project-grid">
  
  <div class="project-card">
    <span class="status-tag tag-done">Completed</span>
    <h3>Akuna Capital: Options 101</h3>
    <p>Deep dive into Options pricing models, The Greeks (Delta/Gamma), and Call/Put parity arbitrage.</p>
    <p><strong>Focus:</strong> Domain Knowledge</p>
  </div>

</div>
