---
layout: archive
title: "Curriculum Vitae"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

<style>
  .cv-section {
    margin: 2.5em 0;
    padding: 1.8em;
    border-radius: 8px;
    box-shadow: 0 4px 12px rgba(0,0,0,0.08);
    background-color: rgba(255,255,255,0.9);
    transition: transform 0.2s, box-shadow 0.2s;
    border-left: 4px solid #3a6a8a;
  }
  .cv-section:hover {
    transform: translateY(-3px);
    box-shadow: 0 6px 18px rgba(0,0,0,0.12);
  }
  .section-heading {
    border-bottom: 2px solid #3a6a8a;
    padding-bottom: 0.5em;
    margin-top: 0;
    margin-bottom: 1em;
    font-size: 1.5em;
    color: #2c3e50;
  }
  .cv-item {
    margin-bottom: 1.2em;
    padding-left: 1.2em;
    position: relative;
    line-height: 1.5;
  }
  .cv-item::before {
    content: "";
    position: absolute;
    left: 0;
    top: 0.5em;
    width: 8px;
    height: 8px;
    background-color: #546e7a;
    border-radius: 50%;
  }
  .cv-degree {
    font-weight: bold;
    color: #2c3e50;
  }
  .cv-institution {
    font-style: italic;
    color: #34495e;
  }
  .cv-date {
    color: #7f8c8d;
    font-size: 0.95em;
  }
  .research-area {
    font-weight: 600;
    color: #2c3e50;
  }
  .cv-list-container {
    background-color: rgba(250,250,250,0.9);
    padding: 1.2em;
    border-left: 3px solid #546e7a;
    margin: 1em 0;
    border-radius: 4px;
    box-shadow: 0 2px 6px rgba(0,0,0,0.05);
  }
  .cv-list-container ul {
    margin-bottom: 0;
  }
  body {
    background-color: #f0f8ff;
    background-attachment: fixed;
  }
</style>

<div class="cv-section">
  <h2 class="section-heading">Education</h2>
  
  <div class="cv-item">
    <span class="cv-degree">Ph.D. in Chemistry</span> | 
    <span class="cv-institution">Hong Kong University of Science and Technology</span> | 
    <span class="cv-date">2023-2027 (expected)</span>
  </div>
  
  <div class="cv-item">
    <span class="cv-degree">M.S. in Chemistry</span> | 
    <span class="cv-institution">Southern University of Science and Technology</span> | 
    <span class="cv-date">2020-2023</span>
  </div>
  
  <div class="cv-item">
    <span class="cv-degree">B.S. in Materials Science and Engineering</span> | 
    <span class="cv-institution">Southern University of Science and Technology</span> | 
    <span class="cv-date">2016-2020</span>
  </div>
</div>

<div class="cv-section">
  <h2 class="section-heading">Research Interests</h2>
  
  <div class="cv-item">
    <span class="research-area">Nano-aggregate Science</span>: Study of nanoscale structures and their properties
  </div>
  
  <div class="cv-item">
    <span class="research-area">Organic Electronics</span>: Investigation of electronic properties in organic materials
  </div>
  
  <div class="cv-item">
    <span class="research-area">Data-centric Scientific Research</span>: Application of data-driven approaches to scientific problems
  </div>
  
  <div class="cv-item">
    <span class="research-area">Electrospun Nanofibers</span>: Development and application of nanofibers produced via electrospinning
  </div>
</div>

<div class="cv-section">
  <h2 class="section-heading">Publications</h2>
  
  <div class="cv-list-container">
    <ul>
      {% for post in site.publications reversed %}
        {% include archive-single-cv.html %}
      {% endfor %}
    </ul>
  </div>
</div>

<div class="cv-section">
  <h2 class="section-heading">Talks</h2>
  
  <div class="cv-list-container">
    <ul>
      {% for post in site.talks reversed %}
        {% include archive-single-talk-cv.html %}
      {% endfor %}
    </ul>
  </div>
</div>

<div class="cv-section">
  <h2 class="section-heading">Teaching</h2>
  
  <div class="cv-list-container">
    <ul>
      {% for post in site.teaching reversed %}
        {% include archive-single-cv.html %}
      {% endfor %}
    </ul>
  </div>
</div>

<div class="cv-section">
  <h2 class="section-heading">Service and Leadership</h2>
  
  <div class="cv-item">
    Currently active in 43 different Slack teams, facilitating academic communication and collaboration
  </div>
</div>
