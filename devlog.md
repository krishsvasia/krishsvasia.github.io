---
layout: default
title: Devlog
permalink: /devlog/
---

<style>
  .project-card {
    background-color: #21262d !important;
    border: 1px solid #30363d;
    border-radius: 12px;
    padding: 25px;
    box-shadow: 0 4px 12px rgba(0,0,0,0.5);
    display: flex;
    flex-direction: column;
    margin-bottom: 30px; /* Space between entries */
    transition: transform 0.2s;
  }

  .project-card:hover {
    transform: translateY(-3px);
    border-color: #58a6ff;
  }

  .project-card h3 {
    margin-top: 10px;
    font-size: 1.4rem;
    color: #ffffff !important;
  }

  .desc-text {
    font-size: 0.95rem;
    color: #8b949e;
    line-height: 1.6;
    margin-bottom: 15px;
  }

  .meta-info {
    font-family: monospace;
    font-size: 0.8rem;
    color: #8b949e;
    margin-bottom: 5px;
  }

  .date-tag {
    color: #58a6ff;
    font-weight: bold;
    margin-right: 10px;
  }

  .read-btn {
    align-self: flex-start;
    margin-top: auto;
    color: #58a6ff;
    text-decoration: none;
    font-weight: bold;
    font-size: 0.9rem;
    border: 1px solid #30363d;
    padding: 8px 16px;
    border-radius: 6px;
    background: #0d1117;
  }

  .read-btn:hover {
    background: #30363d;
    text-decoration: none;
  }
</style>

<h1 style="margin-bottom: 40px; color: white;">Devlog</h1>

<div class="devlog-list">
  
  {% for post in site.posts %}
  <div class="project-card">    
    <div class="meta-info">
      <span class="date-tag">{{ post.date | date: "%b %d, %Y" }}</span>
      <span>{{ post.categories | join: " • " }}</span>
    </div>
    <h3>{{ post.title }}</h3>
    <p class="desc-text">
      {{ post.excerpt | strip_html | truncatewords: 40 }}
    </p>
    <a href="{{ post.url }}" class="read-btn">Read Entry</a>
  </div>
  {% endfor %}

</div>
