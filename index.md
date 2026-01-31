---
layout: default
title: Home
---

<style>
  /* Container for the bottom cards */
  .cards-container {
    margin-top: 60px;
  }

  /* Card Styling */
  .project-card {
    background-color: #21262d !important;
    border: 1px solid #30363d;
    border-radius: 12px;
    padding: 25px;
    box-shadow: 0 4px 12px rgba(0,0,0,0.5);
    display: flex;
    flex-direction: column;
    transition: transform 0.2s;
    margin-bottom: 50px;
  }

  .project-card:hover {
    transform: translateY(-5px);
    border-color: #58a6ff;
  }

  /* Text & Tags inside cards */
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
  .card-link:hover { background: #30363d; }
  
  /* Section Headers for the cards */
  .card-header {
    margin-bottom: 15px;
    color: #c9d1d9;
    font-size: 1.5rem;
    border-bottom: none;
  }
</style>

<div style="margin-bottom: 50px;">
  <h1 style="font-size: 2.5rem; margin-bottom: 20px; color: white;">About Me</h1>

  <p style="font-size: 1.1rem; line-height: 1.8; color: #c9d1d9;">
  I am an Artificial Intelligence and Computer Science student at the University of Birmingham with strong academic performance and I am currently building my experience in development through my own personal projects. I am experienced in collaborative environments and am adaptable through customer-facing roles, improving my communication, teamwork, and problem-solving skills. I am looking forward to learning more about AI and Software Engineering, and aim to become a part of impactful projects related to these in the future.
  </p>

  <div style="margin-top: 25px; padding: 20px; background: #161b22; border: 1px solid #30363d; border-radius: 8px;">
    <p style="margin: 0; line-height: 1.8;">
      <b>Location:</b> Birmingham, UK<br>
      <b>Email:</b> <a href="mailto:krishsvasia@gmail.com">krishsvasia@gmail.com</a><br>
      <b>Links:</b> <a href="https://www.linkedin.com/in/krishvasia/">LinkedIn</a> | <a href="https://github.com/krishsvasia">GitHub</a> | <a href="./CV.pdf">Download CV</a>
    </p>
  </div>
</div>

<div style="margin-top: 30px; display: flex; gap: 30px; flex-wrap: wrap;">

  <div style="flex: 1; min-width: 300px;">
    <h3 style="color: white; border-bottom: 1px solid #30363d; padding-bottom: 10px; margin-bottom: 15px;">Education</h3> 
    <div style="margin-bottom: 15px;">
      <strong style="color: #c9d1d9; font-size: 1.1rem;">BSc Artificial Intelligence & Computer Science</strong><br>
      <span style="color: #8b949e;">University of Birmingham</span>
    </div>
    <div>
      <strong style="color: #c9d1d9; font-size: 1.1rem;">A-Levels</strong><br>
      <span style="color: #8b949e; font-size: 0.9rem;">
       Mathematics (A), Computer Science (A), Physics (A)
      </span>
    </div>
  </div>

  <div style="flex: 1; min-width: 300px;">
    <h3 style="color: white; border-bottom: 1px solid #30363d; padding-bottom: 10px; margin-bottom: 15px;">Awards</h3>     
    <div style="margin-bottom: 15px;">
      <strong style="color: #c9d1d9;">Senior Kangaroo Qualifier</strong><br>
      <span style="color: #8b949e; font-size: 0.9rem;">
       Invited merit round for high scorers.
      </span>
    </div>
    <div>
      <strong style="color: #c9d1d9;">3x UKMT Maths Challenge Gold Award</strong><br>
      <span style="color: #8b949e; font-size: 0.9rem;">
       Top 8% of participants nationwide.
      </span>
    </div>
  </div>

</div>

<hr style="border-color: #30363d; margin: 40px 0;">

<div class="cards-container">

  <h2 class="card-header">Current Program Focus</h2>
  <div class="project-card">
    <div>
      <span class="status-tag tag-wip">In Progress</span>
      <h3>Adaptive Kalman Filter</h3>
      <p class="desc-text">
        Statistical arbitrage engine using a Kalman Filter to track the relationship between two tickers on the market. Currently adding more features, such as and adaptive noise algorithm for learning.
      </p>
      <p class="tech-stack">Python • Pandas • NumPy</p>
    </div>
    <a href="/projects/" class="card-link">View Projects</a>
  </div>

  <h2 class="card-header">Latest Devlog</h2>
  <div class="project-card">
    <div>
      <span class="status-tag tag-new">Jan 31, 2026</span>
      <h3>Devlog 0: Setting the Foundation</h3>
      <p class="desc-text">
        My first weekly log. Reflections on completing the Akuna Options 101 course, my roadmap for learning C++26, and plans for my Kalman Filter.
      </p>
      <p class="tech-stack">Journal • C++ • Finance</p>
    </div>
    <a href="/devlog" class="card-link">View Devlogs</a>
  </div>

</div>
