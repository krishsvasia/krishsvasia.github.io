---
layout: default
title: Projects
permalink: /projects/
---

<style>
  /* 1. The Container: 3 Columns */
  .project-grid {
    display: grid;
    /* Forces exactly 3 equal columns. */
    /* minmax(250px, 1fr) means they won't get smaller than 250px before stacking. */
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 25px; /* Nice spacing between cards */
    margin-bottom: 40px;
  }

  /* 2. The Cards: Dark Mode & Aesthetics */
  .project-card {
    /* DARK MODE COLORS */
    background-color: #161b22; /* Deep dark grey */
    border: 1px solid #30363d; /* Subtle dark border */
    
    /* SHAPE & SPACING ("Less Rectangular") */
    border-radius: 16px; /* Very round corners */
    padding: 25px; /* internal breathing room */
    box-shadow: 0 4px 12px rgba(0,0,0,0.2); /* Soft shadow for depth */
    
    /* LAYOUT */
    display: flex;
    flex-direction: column;
    height: 100%; /* Ensures cards in the same row are equal height */
    transition: all 0.2s ease-in-out;
  }

  /* Hover Effect: Pop up and glow blue */
  .project-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 12px 20px rgba(0,0,0,0.3);
    border-color: #58a6ff; /* GitHub Blue highlight */
  }

  /* 3. Typography Controls */
  .project-card h3 {
    margin-top: 15px;
    margin-bottom: 10px;
    font-size: 1.25rem;
    color: #ffffff; /* Bright white titles */
  }

  /* SMALLER DESCRIPTION TEXT */
  .desc-text {
    font-size: 0.9rem; /* Smaller than normal text */
    line-height: 1.5;
    color: #8b949e; /* Slightly dimmed text */
    flex-grow: 1; /* Pushes the link button to the bottom */
    margin-bottom: 20px;
  }

  /* Tech Stack text */
  .tech-stack {
    font-size: 0.85rem;
    font-weight: bold;
    color: #c9d1d9;
    margin-bottom: 15px;
  }

  /* 4. Tags & Buttons */
  .status-tag {
    display: inline-block;
    padding: 4px 10px;
    border-radius: 20px; /* Capsule shape */
    font-size: 0.75em;
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: 0.5px;
  }
  
  /* Tag Colors for Dark Mode */
  .tag-wip { background: rgba(210, 153, 34, 0.2); color: #d29922; border: 1px solid #d29922; }
  .tag-planned { background: rgba(139, 148, 158, 0.2); color: #8b949e; border: 1px solid #8b949e; }
  .tag-done { background: rgba(46, 160, 67, 0.2); color: #3fb950; border: 1px solid #3fb950; }

  /* Custom Link Button */
  .card-link {
    display: block;
    text-align: center;
    background: #21262d;
    color: #58a6ff;
    padding: 10px;
    border-radius: 8px;
    text-decoration: none;
    font-weight: bold;
    border: 1px solid #30363d;
  }
  .card-link:hover { background: #30363d; }

</style>

<h2>🚀 Engineering Projects</h2>

<div class="project-grid">

  <div class="project-card">
    <div>
      <span class="status-tag tag-wip">In Progress</span>
      <h3>Zero-Copy Parser</h3>
      <p class="desc-text">High-throughput C++20 library for parsing ITCH binary market data. Benchmarking <code>mmap</code> vs standard I/O.</p>
      <p class="tech-stack">C++26 • Linux API • Perf</p>
    </div>
    <a href="#" class="card-link">View Code →</a>
  </div>

  <div class="project-card">
      <div>
        <span class="status-tag tag-wip">Completed</span>
        <h3>Vector Kalman Filter</h3>
        <p class="desc-text">Statistical arbitrage strategy using EM algorithm for noise learning.</p>
        <p class="tech-stack">Python, Pandas, NumPy</p>
      </div>
      <a href="#" class="card-link">View Research →</a>
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
  </div>

</div>
