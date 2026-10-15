---
layout: archive
title: "Publications"
title_zh: "学术论文"
permalink: /publications/
author_profile: true
academic_style: true
---

<div class="publications-container">
  {% if site.author.googlescholar %}
    <div class="scholar-link">
      <span class="lang-en">You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</span>
      <span class="lang-zh">你也可以在<a href="{{site.author.googlescholar}}">我的 Google Scholar 主页</a>上查看我的文章。</span>
    </div>
  {% endif %}

  <h2 class="section-heading"><span class="lang-en">Articles and Patents</span><span class="lang-zh">论文与专利</span></h2>

  {% include base_path %}

  {% assign publications_by_year = site.publications | group_by_exp: "post", "post.date | date: '%Y'" %}
  {% assign sorted_years = publications_by_year | sort: "name" | reverse %}

  {% for year_group in sorted_years %}
    <h3 class="year-heading">{{ year_group.name }}</h3>
    {% for post in year_group.items %}
      <div class="pub-item">
        {% include archive-single.html %}
      </div>
    {% endfor %}
  {% endfor %}
</div>
