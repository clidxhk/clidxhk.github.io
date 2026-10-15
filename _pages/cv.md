---
layout: archive
title: "Curriculum Vitae"
permalink: /cv/
author_profile: true
academic_style: true
redirect_from:
  - /resume
  - /service/
  - /service.html
---

{% include base_path %}

<div class="academic-panel">
<section class="cv-section" aria-labelledby="cv-edu">
  <p class="cv-eyebrow">Background</p>
  <h2 class="cv-heading" id="cv-edu">Education</h2>
  <div class="cv-grid cv-grid--3">
    <article class="cv-card">
      <span class="cv-icon"><i class="fas fa-graduation-cap" aria-hidden="true"></i></span>
      <h3>Ph.D. in Chemistry</h3>
      <p>The Hong Kong University of Science and Technology</p>
      <p class="cv-meta">2023&ndash;present (expected 2027)</p>
      <p class="cv-advisor">Advisors: Prof. Ben-Zhong Tang and Prof. Sun</p>
    </article>
    <article class="cv-card">
      <span class="cv-icon"><i class="fas fa-flask" aria-hidden="true"></i></span>
      <h3>M.S. in Chemistry</h3>
      <p>Southern University of Science and Technology</p>
      <p class="cv-meta">2020&ndash;2023</p>
      <p class="cv-advisor">Advisor: Prof. Kai Li</p>
    </article>
    <article class="cv-card">
      <span class="cv-icon"><i class="fas fa-atom" aria-hidden="true"></i></span>
      <h3>B.S. in Materials Science and Engineering</h3>
      <p>Southern University of Science and Technology</p>
      <p class="cv-meta">2016&ndash;2020</p>
    </article>
  </div>
</section>

<section class="cv-section" aria-labelledby="cv-interests">
  <p class="cv-eyebrow">Focus</p>
  <h2 class="cv-heading" id="cv-interests">Research Interests</h2>
  <div class="cv-grid cv-grid--2">
    <article class="cv-card">
      <span class="cv-icon"><i class="fas fa-lightbulb" aria-hidden="true"></i></span>
      <h3>Photodynamic Therapy &amp; AIE Photosensitizers</h3>
      <p>Rational design of aggregation-induced emission photosensitizers for anti-tumor and anti-pathogen applications.</p>
    </article>
    <article class="cv-card">
      <span class="cv-icon"><i class="fas fa-eye" aria-hidden="true"></i></span>
      <h3>Biomedical Photochemistry</h3>
      <p>Advanced imaging technologies, image-guided therapy and remote phototherapy with excited-state molecules.</p>
    </article>
    <article class="cv-card">
      <span class="cv-icon"><i class="fas fa-brain" aria-hidden="true"></i></span>
      <h3>AI for Chemistry</h3>
      <p>Data-driven molecular engineering and machine-learning-guided discovery of functional photosensitizers.</p>
    </article>
    <article class="cv-card">
      <span class="cv-icon"><i class="fas fa-layer-group" aria-hidden="true"></i></span>
      <h3>Functional Fibrous Materials</h3>
      <p>Electrospun anti-pathogen fibrous membranes for textile and medical applications.</p>
    </article>
  </div>
</section>

<section class="cv-section" aria-labelledby="cv-pubs">
  <p class="cv-eyebrow">Scholarship</p>
  <h2 class="cv-heading" id="cv-pubs">Publications</h2>
  <div class="cv-card">
    <ul class="cv-entries">
      {% for post in site.publications reversed %}
        {% unless post.type == "Patent" %}
          {% include archive-single-cv.html %}
        {% endunless %}
      {% endfor %}
    </ul>
  </div>
</section>

<section class="cv-section" aria-labelledby="cv-patents">
  <p class="cv-eyebrow">Innovation</p>
  <h2 class="cv-heading" id="cv-patents">Patents</h2>
  <div class="cv-card">
    <ul class="cv-entries">
      {% for post in site.publications reversed %}
        {% if post.type == "Patent" %}
          {% include archive-single-cv.html %}
        {% endif %}
      {% endfor %}
    </ul>
  </div>
</section>

<section class="cv-section" aria-labelledby="cv-software">
  <p class="cv-eyebrow">Tools</p>
  <h2 class="cv-heading" id="cv-software">Software</h2>
  <div class="cv-card">
    <span class="cv-icon"><i class="fas fa-calculator" aria-hidden="true"></i></span>
    <h3>Solvent Fraction Convertor</h3>
    <p>A web tool for interconverting the mole, volume and mass fractions of solvent mixtures.</p>
    <div class="cv-buttons">
      <a class="cv-button cv-button--primary" href="https://clidx-solvent-fraction-convertor.hf.space">Hugging Face <i class="fas fa-arrow-right" aria-hidden="true"></i></a>
      <a class="cv-button cv-button--secondary" href="https://modelscope.cn/studios/SUSTechCN/Solvent_Fraction_Convertor/summary">ModelScope 魔搭</a>
    </div>
  </div>
</section>

<section class="cv-section" aria-labelledby="cv-prizes">
  <p class="cv-eyebrow">Recognition</p>
  <h2 class="cv-heading" id="cv-prizes">Prizes</h2>
  <div class="cv-card">
    <ul class="cv-entries">
      {% for post in site.prizes reversed %}
        {% include archive-single-cv.html %}
      {% endfor %}
    </ul>
  </div>
</section>

<section class="cv-section" aria-labelledby="cv-teaching">
  <p class="cv-eyebrow">Experience</p>
  <h2 class="cv-heading" id="cv-teaching">Teaching</h2>
  <div class="cv-card">
    <ul class="cv-entries">
      {% for post in site.teaching reversed %}
        {% include archive-single-cv.html %}
      {% endfor %}
    </ul>
  </div>
</section>

<section class="cv-section" aria-labelledby="cv-service">
  <p class="cv-eyebrow">Community</p>
  <h2 class="cv-heading" id="cv-service">Service</h2>
  <div class="cv-statement">
    <div>
      <h3>Volunteering &amp; giving</h3>
      <p>Community service and charitable giving alongside research.</p>
    </div>
    <div>
      <p><strong>58.67 hours</strong> of volunteer service</p>
      <p><strong>RMB 8,440.02</strong> in cumulative charitable donations</p>
    </div>
  </div>
</section>

</div>
