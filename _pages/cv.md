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
  .cv-section { margin: 0 0 4rem; }
  .cv-eyebrow { margin: 0 0 .6rem; color: #50bdba; font-size: .78em; font-weight: 700; letter-spacing: .14em; text-transform: uppercase; }
  .cv-heading { max-width: 650px; margin: 0 0 1.8rem; color: #133248; font-size: clamp(1.7rem, 3.5vw, 2.4rem); font-weight: 700; letter-spacing: -.03em; line-height: 1.18; }

  .cv-grid { display: grid; gap: 1rem; }
  .cv-grid--3 { grid-template-columns: repeat(3, 1fr); }
  .cv-grid--2 { grid-template-columns: repeat(2, 1fr); }

  .cv-card { padding: 1.55rem; border: 1px solid #dce8eb; border-radius: .75rem; background: #fff; box-shadow: 0 8px 24px rgba(15,53,70,.05); transition: transform .2s ease, box-shadow .2s ease; }
  .cv-card:hover { transform: translateY(-4px); box-shadow: 0 16px 30px rgba(15,53,70,.11); }

  .cv-icon { display: inline-grid; width: 2.6rem; height: 2.6rem; place-items: center; border-radius: .55rem; color: #147a82; background: #e5f5f3; font-size: 1.05rem; }
  .cv-card h3 { margin: 1.05rem 0 .55rem; color: #143449; font-size: 1.08em; line-height: 1.3; }
  .cv-card p { margin: 0 0 .45rem; color: #617586; font-size: .9em; line-height: 1.6; }
  .cv-card .cv-meta { color: #78909c; font-size: .84em; }
  .cv-card .cv-advisor { color: #617586; font-size: .86em; }

  .cv-entries { margin: 0; padding: 0; list-style: none; }
  .cv-entries .archive__item { margin: 0; padding: 1.05rem 0; border-bottom: 1px solid #e6eff2; }
  .cv-entries .archive__item:first-child { padding-top: .3rem; }
  .cv-entries .archive__item:last-child { padding-bottom: .35rem; border-bottom: none; }
  .cv-entries .archive__item-title { margin: 0 0 .3rem; font-size: 1.02em; }
  .cv-entries .archive__item-excerpt { margin: 0; color: #617586; font-size: .9em; line-height: 1.65; }

  .cv-statement { display: grid; grid-template-columns: 1.05fr .95fr; gap: 3rem; padding: clamp(1.6rem, 4vw, 2.8rem); border-left: 4px solid #35a6a3; background: #edf6f6; border-radius: 0 .75rem .75rem 0; }
  .cv-statement > div { align-self: center; }
  .cv-statement h3 { margin: 0 0 .4rem; color: #143449; font-size: 1.15em; }
  .cv-statement p { margin: 0; color: #36576a; font-size: .98em; line-height: 1.75; }

  .cv-buttons { display: flex; flex-wrap: wrap; gap: .75rem; margin-top: 1.1rem; }
  .cv-button { display: inline-flex; align-items: center; gap: .55rem; padding: .68rem 1.05rem; border: 1px solid transparent; border-radius: .35rem; font-size: .88em; font-weight: 700; text-decoration: none; transition: transform .2s ease, background-color .2s ease; }
  .cv-button:hover { transform: translateY(-2px); }
  .cv-button--primary { color: #0b2a3c; background: #d2efeb; }
  .cv-button--primary:hover { color: #071b27; background: #fff; }
  .cv-button--secondary { color: #0b2a3c; border-color: #9ecfd2; }
  .cv-button--secondary:hover { background: rgba(255,255,255,.6); }

  @media (max-width: 900px) {
    .cv-grid--3, .cv-grid--2 { grid-template-columns: 1fr; }
    .cv-statement { grid-template-columns: 1fr; gap: 1.3rem; }
  }
</style>

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
      <p><strong style="color:#143449">58.67 hours</strong> of volunteer service</p>
      <p><strong style="color:#143449">RMB 8,440.02</strong> in cumulative charitable donations</p>
    </div>
  </div>
</section>
