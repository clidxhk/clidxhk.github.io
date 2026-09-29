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
  .cv-advisor {
    display: block;
    color: #7f8c8d;
    font-size: 0.95em;
  }
  .research-area {
    font-weight: 600;
    color: #2c3e50;
  }
  .cv-list-container {
    background-color: rgba(250,250,250,0.9);
    padding: 1.2em 1.4em;
    border-left: 3px solid #546e7a;
    margin: 1em 0;
    border-radius: 4px;
    box-shadow: 0 2px 6px rgba(0,0,0,0.05);
  }
  .cv-list-container ul {
    margin: 0;
    padding-left: 0;
    list-style: none;
  }
  .cv-list-container li.archive__item {
    margin: 0 0 1.2em 0;
  }
  .cv-list-container li.archive__item:last-child {
    margin-bottom: 0;
  }
  .cv-list-container .archive__item-title {
    margin: 0 0 0.25em 0;
  }
  .cv-list-container .archive__item-excerpt {
    margin: 0;
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
    <span class="cv-institution">The Hong Kong University of Science and Technology</span> |
    <span class="cv-date">2023&ndash;present (expected 2027)</span>
    <span class="cv-advisor">Advisors: Prof. Ben-Zhong Tang and Prof. Sun</span>
  </div>

  <div class="cv-item">
    <span class="cv-degree">M.S. in Chemistry</span> |
    <span class="cv-institution">Southern University of Science and Technology</span> |
    <span class="cv-date">2020&ndash;2023</span>
    <span class="cv-advisor">Advisor: Prof. Kai Li</span>
  </div>

  <div class="cv-item">
    <span class="cv-degree">B.S. in Materials Science and Engineering</span> |
    <span class="cv-institution">Southern University of Science and Technology</span> |
    <span class="cv-date">2016&ndash;2020</span>
  </div>
</div>

<div class="cv-section">
  <h2 class="section-heading">Research Interests</h2>

  <div class="cv-item">
    <span class="research-area">Photodynamic Therapy &amp; AIE Photosensitizers</span>: Rational design of aggregation-induced emission photosensitizers for anti-tumor and anti-pathogen applications
  </div>

  <div class="cv-item">
    <span class="research-area">Biomedical Photochemistry</span>: Advanced imaging technologies, image-guided therapy and remote phototherapy with excited-state molecules
  </div>

  <div class="cv-item">
    <span class="research-area">AI for Chemistry</span>: Data-driven molecular engineering and machine-learning-guided discovery of functional photosensitizers
  </div>

  <div class="cv-item">
    <span class="research-area">Functional Fibrous Materials</span>: Electrospun anti-pathogen fibrous membranes for textile and medical applications
  </div>
</div>

<div class="cv-section">
  <h2 class="section-heading">Publications</h2>

  <div class="cv-list-container">
    <ul>
      {% for post in site.publications reversed %}
        {% unless post.type == "Patent" %}
          {% include archive-single-cv.html %}
        {% endunless %}
      {% endfor %}
    </ul>
  </div>
</div>

<div class="cv-section">
  <h2 class="section-heading">Patents</h2>

  <div class="cv-list-container">
    <ul>
      {% for post in site.publications reversed %}
        {% if post.type == "Patent" %}
          {% include archive-single-cv.html %}
        {% endif %}
      {% endfor %}
    </ul>
  </div>
</div>

<div class="cv-section">
  <h2 class="section-heading">Software</h2>

  <div class="cv-item">
    <span class="research-area">Solvent Fraction Convertor</span> (2025): A web tool for interconverting the mole, volume and mass fractions of solvent mixtures.
    <br>
    <a href="https://clidx-solvent-fraction-convertor.hf.space">Hugging Face</a> &middot; <a href="https://modelscope.cn/studios/SUSTechCN/Solvent_Fraction_Convertor/summary">ModelScope (魔搭)</a>
  </div>
</div>

<div class="cv-section">
  <h2 class="section-heading">Prizes</h2>

  <div class="cv-list-container">
    <ul>
      {% for post in site.prizes reversed %}
        {% include archive-single-cv.html %}
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
  <h2 class="section-heading">Service</h2>

  <div class="cv-item">
    Volunteer service: 58.67 hours
  </div>

  <div class="cv-item">
    Cumulative charitable donations: RMB 8,440.02
  </div>
</div>
