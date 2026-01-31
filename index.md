---
layout: default
title: Home
---

<style>
  /* --- Homepage Specific Styles --- */

  /* Centers the content and limits width */
  .home-container {
    max-width: 800px;
    margin: 0 auto; 
  }

  /* Card Styling (Matches Projects Page) */
  .project-card {
    background-color: #21262d !important;
    border: 1px solid #30363d;
    border-radius: 12px;
    padding: 25px;
    box-shadow: 0 4px 12px rgba(0,0,0,0.5);
    display: flex;
    flex-direction: column;
    transition: transform 0.2s;
    margin-bottom: 50px; /* Space between the two sections */
  }

  .project-card:hover {
    transform: translateY(-5px);
    border-color: #58a6ff;
  }

  /* Headings */
  h2 {
    margin-bottom: 15px;
    border-bottom: none; /* Removes default Jekyll underline */
    color: #c9d1d9;
  }

  /* Text Styles */
  .project-card h3 {
    margin-top: 15px;
    font-size: 1.4rem;
    color: #ffffff !important;
  }

  .desc-text {
    font-size: 0.95rem;
    color: #8b949e;
    line-height: 1.5;
    margin-bottom: 15px;
  }

  .tech-stack {
    font-size: 0.85rem;
    font-weight: bold;
    color: #c9d1d9;
  }

  /* Tags */
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
  .tag-new { background: rgba(88, 166, 255, 0.15); color: #58a6ff; border: 1px solid #58a6ff; }

  /* Buttons */
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
    margin-top: 20px;
  }
  .card-link:hover { 
    background: #30363d; 
  }
</style>

<div class="home-container">

  <h2>Current Program Focus</h2>
  <div class="project-card">
    <div>
      <span class="status-tag tag-wip">In Progress</span>
      <h3>Systems Programming</h3>
      <p class="desc-text">
        Deep dive into C++20 memory management. Currently building a Zero-Copy Parser for ITCH market data to minimize latency.
      </p>
      <p class="tech-stack">C++ • Pointers • Linux API</p>
    </div>
    <a href="/projects/" class="card-link">View Roadmap</a>
  </div>

  <h2>Latest Devlog</h2>
  <div class="project-card">
    <div>
      <span class="status-tag tag-new">Jan 30, 2026</span>
      <h3>Building a Zero-Copy Parser</h3>
      <p class="desc-text">
        Optimizing memory access by eliminating redundant data copying. A look into <code>mmap</code> vs standard I/O performance.
      </p>
      <p class="tech-stack">Systems • Optimization</p>
    </div>
    <a href="/devlog/building-zero-copy-parser" class="card-link">Read Entry</a>
  </div>

</div>
