---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
academic_style: true
---

<div class="publications-container">
  {% if site.author.googlescholar %}
    <div class="scholar-link">
      You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.
    </div>
  {% endif %}

  <h2 class="section-heading">Articles and Patents</h2>

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
