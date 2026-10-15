---
layout: archive
title: "Curriculum Vitae"
title_zh: "简历"
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
  <p class="cv-eyebrow"><span class="lang-en">Background</span><span class="lang-zh">背景</span></p>
  <h2 class="cv-heading" id="cv-edu"><span class="lang-en">Education</span><span class="lang-zh">教育经历</span></h2>
  <div class="cv-grid cv-grid--3">
    <article class="cv-card">
      <span class="cv-icon"><i class="fas fa-graduation-cap" aria-hidden="true"></i></span>
      <h3><span class="lang-en">Ph.D. in Chemistry</span><span class="lang-zh">化学博士</span></h3>
      <p><span class="lang-en">The Hong Kong University of Science and Technology</span><span class="lang-zh">香港科技大学</span></p>
      <p class="cv-meta"><span class="lang-en">2023&ndash;present (expected 2027)</span><span class="lang-zh">2023&ndash;至今（预计 2027 年毕业）</span></p>
      <p class="cv-advisor"><span class="lang-en">Advisors: Prof. Ben-Zhong Tang and Prof. Sun</span><span class="lang-zh">导师：唐本忠教授、孙教授</span></p>
    </article>
    <article class="cv-card">
      <span class="cv-icon"><i class="fas fa-flask" aria-hidden="true"></i></span>
      <h3><span class="lang-en">M.S. in Chemistry</span><span class="lang-zh">化学硕士</span></h3>
      <p><span class="lang-en">Southern University of Science and Technology</span><span class="lang-zh">南方科技大学</span></p>
      <p class="cv-meta">2020&ndash;2023</p>
      <p class="cv-advisor"><span class="lang-en">Advisor: Prof. Kai Li</span><span class="lang-zh">导师：李凯教授</span></p>
    </article>
    <article class="cv-card">
      <span class="cv-icon"><i class="fas fa-atom" aria-hidden="true"></i></span>
      <h3><span class="lang-en">B.S. in Materials Science and Engineering</span><span class="lang-zh">材料科学与工程学士</span></h3>
      <p><span class="lang-en">Southern University of Science and Technology</span><span class="lang-zh">南方科技大学</span></p>
      <p class="cv-meta">2016&ndash;2020</p>
    </article>
  </div>
</section>

<section class="cv-section" aria-labelledby="cv-interests">
  <p class="cv-eyebrow"><span class="lang-en">Focus</span><span class="lang-zh">聚焦</span></p>
  <h2 class="cv-heading" id="cv-interests"><span class="lang-en">Research Interests</span><span class="lang-zh">研究兴趣</span></h2>
  <div class="cv-grid cv-grid--2">
    <article class="cv-card">
      <span class="cv-icon"><i class="fas fa-lightbulb" aria-hidden="true"></i></span>
      <h3><span class="lang-en">Photodynamic Therapy &amp; AIE Photosensitizers</span><span class="lang-zh">光动力治疗与 AIE 光敏剂</span></h3>
      <p><span class="lang-en">Rational design of aggregation-induced emission photosensitizers for anti-tumor and anti-pathogen applications.</span><span class="lang-zh">面向抗肿瘤与抗病原体应用的聚集诱导发光（AIE）光敏剂的合理设计。</span></p>
    </article>
    <article class="cv-card">
      <span class="cv-icon"><i class="fas fa-eye" aria-hidden="true"></i></span>
      <h3><span class="lang-en">Biomedical Photochemistry</span><span class="lang-zh">生物医学光化学</span></h3>
      <p><span class="lang-en">Advanced imaging technologies, image-guided therapy and remote phototherapy with excited-state molecules.</span><span class="lang-zh">先进成像技术、图像引导治疗及基于激发态分子的远程光疗。</span></p>
    </article>
    <article class="cv-card">
      <span class="cv-icon"><i class="fas fa-brain" aria-hidden="true"></i></span>
      <h3><span class="lang-en">AI for Chemistry</span><span class="lang-zh">人工智能 × 化学</span></h3>
      <p><span class="lang-en">Data-driven molecular engineering and machine-learning-guided discovery of functional photosensitizers.</span><span class="lang-zh">数据驱动的分子工程与机器学习引导的功能光敏剂发现。</span></p>
    </article>
    <article class="cv-card">
      <span class="cv-icon"><i class="fas fa-layer-group" aria-hidden="true"></i></span>
      <h3><span class="lang-en">Functional Fibrous Materials</span><span class="lang-zh">功能纤维材料</span></h3>
      <p><span class="lang-en">Electrospun anti-pathogen fibrous membranes for textile and medical applications.</span><span class="lang-zh">面向纺织与医疗应用的静电纺丝抗病原体纤维膜。</span></p>
    </article>
  </div>
</section>

<section class="cv-section" aria-labelledby="cv-pubs">
  <p class="cv-eyebrow"><span class="lang-en">Scholarship</span><span class="lang-zh">学术</span></p>
  <h2 class="cv-heading" id="cv-pubs"><span class="lang-en">Publications</span><span class="lang-zh">学术论文</span></h2>
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
  <p class="cv-eyebrow"><span class="lang-en">Innovation</span><span class="lang-zh">创新</span></p>
  <h2 class="cv-heading" id="cv-patents"><span class="lang-en">Patents</span><span class="lang-zh">专利</span></h2>
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

<section class="cv-section" aria-labelledby="cv-prizes">
  <p class="cv-eyebrow"><span class="lang-en">Recognition</span><span class="lang-zh">荣誉</span></p>
  <h2 class="cv-heading" id="cv-prizes"><span class="lang-en">Prizes</span><span class="lang-zh">奖项</span></h2>
  <div class="cv-card">
    <ul class="cv-entries">
      {% for post in site.prizes reversed %}
        {% include archive-single-cv.html %}
      {% endfor %}
    </ul>
  </div>
</section>

<section class="cv-section" aria-labelledby="cv-teaching">
  <p class="cv-eyebrow"><span class="lang-en">Experience</span><span class="lang-zh">经历</span></p>
  <h2 class="cv-heading" id="cv-teaching"><span class="lang-en">Teaching</span><span class="lang-zh">教学</span></h2>
  <div class="cv-card">
    <ul class="cv-entries">
      {% for post in site.teaching reversed %}
        {% include archive-single-cv.html %}
      {% endfor %}
    </ul>
  </div>
</section>

<section class="cv-section" aria-labelledby="cv-service">
  <p class="cv-eyebrow"><span class="lang-en">Community</span><span class="lang-zh">公益</span></p>
  <h2 class="cv-heading" id="cv-service"><span class="lang-en">Service</span><span class="lang-zh">社会服务</span></h2>
  <div class="cv-statement">
    <div>
      <h3><span class="lang-en">Volunteering &amp; giving</span><span class="lang-zh">志愿服务与公益捐赠</span></h3>
      <p><span class="lang-en">Community service and charitable giving alongside research.</span><span class="lang-zh">在科研之外参与社区服务与慈善捐赠。</span></p>
    </div>
    <div>
      <p><span class="lang-en"><strong>58.67 hours</strong> of volunteer service</span><span class="lang-zh"><strong>58.67 小时</strong>志愿服务</span></p>
      <p><span class="lang-en"><strong>RMB 8,440.02</strong> in cumulative charitable donations</span><span class="lang-zh">累计慈善捐赠 <strong>8,440.02 元</strong>人民币</span></p>
    </div>
  </div>
</section>

</div>
