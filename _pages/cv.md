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
  .cv-section { margin: 0 0 3.25rem; }
  .cv-eyebrow { margin: 0 0 .5rem; color: #35a6a3; font-size: .75em; font-weight: 700; letter-spacing: .14em; text-transform: uppercase; }
  .cv-heading { margin: 0 0 1.6rem; color: #133248; font-size: clamp(1.55rem, 3vw, 2.05rem); letter-spacing: -.02em; line-height: 1.2; }
  .cv-item { margin: 0 0 1.1rem; padding: 0 0 1.1rem; border-bottom: 1px solid #dce8eb; }
  .cv-item:last-child { margin: 0; padding: 0; border-bottom: none; }
  .cv-degree, .research-area { font-weight: 700; color: #143449; }
  .cv-institution { color: #36576a; }
  .cv-date { color: #78909c; font-size: .92em; }
  .cv-advisor { display: block; margin-top: .2rem; color: #617586; font-size: .92em; }
  .cv-entries { margin: 0; padding: 0; list-style: none; }
  .cv-entries .archive__item { margin: 0 0 1.15rem; padding: 0 0 1.15rem; border-bottom: 1px solid #dce8eb; }
  .cv-entries .archive__item:last-child { margin: 0; padding: 0; border-bottom: none; }
  .cv-entries .archive__item-title { margin: 0 0 .3rem; font-size: 1.05em; }
  .cv-entries .archive__item-excerpt { margin: 0; color: #617586; font-size: .92em; line-height: 1.65; }
</style>

<section class="cv-section" aria-labelledby="cv-edu">
  <p class="cv-eyebrow">Background</p>
  <h2 class="cv-heading" id="cv-edu">Education</h2>

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
</section>

<section class="cv-section" aria-labelledby="cv-interests">
  <p class="cv-eyebrow">Focus</p>
  <h2 class="cv-heading" id="cv-interests">Research Interests</h2>

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
</section>

<section class="cv-section" aria-labelledby="cv-pubs">
  <p class="cv-eyebrow">Scholarship</p>
  <h2 class="cv-heading" id="cv-pubs">Publications</h2>

  <ul class="cv-entries">
    {% for post in site.publications reversed %}
      {% unless post.type == "Patent" %}
        {% include archive-single-cv.html %}
      {% endunless %}
    {% endfor %}
  </ul>
</section>

<section class="cv-section" aria-labelledby="cv-patents">
  <p class="cv-eyebrow">Innovation</p>
  <h2 class="cv-heading" id="cv-patents">Patents</h2>

  <ul class="cv-entries">
    {% for post in site.publications reversed %}
      {% if post.type == "Patent" %}
        {% include archive-single-cv.html %}
      {% endif %}
    {% endfor %}
  </ul>
</section>

<section class="cv-section" aria-labelledby="cv-software">
  <p class="cv-eyebrow">Tools</p>
  <h2 class="cv-heading" id="cv-software">Software</h2>

  <div class="cv-item">
    <span class="research-area">Solvent Fraction Convertor</span> (2025): A web tool for interconverting the mole, volume and mass fractions of solvent mixtures.
    <br>
    <a href="https://clidx-solvent-fraction-convertor.hf.space">Hugging Face</a> &middot; <a href="https://modelscope.cn/studios/SUSTechCN/Solvent_Fraction_Convertor/summary">ModelScope (魔搭)</a>
  </div>
</section>

<section class="cv-section" aria-labelledby="cv-prizes">
  <p class="cv-eyebrow">Recognition</p>
  <h2 class="cv-heading" id="cv-prizes">Prizes</h2>

  <ul class="cv-entries">
    {% for post in site.prizes reversed %}
      {% include archive-single-cv.html %}
    {% endfor %}
  </ul>
</section>

<section class="cv-section" aria-labelledby="cv-teaching">
  <p class="cv-eyebrow">Experience</p>
  <h2 class="cv-heading" id="cv-teaching">Teaching</h2>

  <ul class="cv-entries">
    {% for post in site.teaching reversed %}
      {% include archive-single-cv.html %}
    {% endfor %}
  </ul>
</section>

<section class="cv-section" aria-labelledby="cv-service">
  <p class="cv-eyebrow">Community</p>
  <h2 class="cv-heading" id="cv-service">Service</h2>

  <div class="cv-item">
    Volunteer service: 58.67 hours
  </div>

  <div class="cv-item">
    Cumulative charitable donations: RMB 8,440.02
  </div>
</section>
