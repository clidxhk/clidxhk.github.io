---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

<style>
  .publications-header {
    margin: 2.5em 0 1.5em 0;
    padding: 1.8em;
    border-radius: 4px;
    box-shadow: 0 1px 3px rgba(0,0,0,0.1);
    background-color: #f9f9f9;
  }
  .section-heading {
    border-bottom: 2px solid #3a6a8a;
    padding-bottom: 0.5em;
    margin-top: 0;
    margin-bottom: 1em;
    font-size: 1.5em;
    color: #333;
  }
  .article-item {
    margin: 2em 0;
    padding: 1.5em;
    border-radius: 4px;
    box-shadow: 0 1px 3px rgba(0,0,0,0.1);
    background-color: #f9f9f9;
  }
  .article-item:hover {
    box-shadow: 0 2px 5px rgba(0,0,0,0.15);
    transition: box-shadow 0.3s ease;
  }
  .scholar-link {
    margin-bottom: 1em;
    font-size: 0.95em;
  }
  .scholar-link a {
    font-weight: 600;
    text-decoration: underline;
    color: #34495e;
  }
  .year-divider {
    margin: 2.5em 0 1em 0;
    padding-bottom: 0.5em;
    font-size: 1.2em;
    color: #3a6a8a;
    border-bottom: 1px solid #ddd;
  }
</style>

<div class="publications-header">
  <h2 class="section-heading">Research Articles</h2>
  
  {% if site.author.googlescholar %}
    <p class="scholar-link">You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</p>
  {% endif %}
</div>

{% include base_path %}

{% assign grouped_publications = site.publications | group_by_exp: "post", "post.date | date: '%Y'" %}
{% for year in grouped_publications %}
  <div class="year-divider">{{ year.name }}</div>
  {% for post in year.items %}
    <div class="article-item">
      {% include archive-single.html %}
    </div>
  {% endfor %}
{% endfor %}
