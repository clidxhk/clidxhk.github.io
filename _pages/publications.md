---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

<style>
  .publications-container {
    margin: 1.5em 0;
    padding: 1em;
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
  .pub-item {
    margin: 0.8em 0;
    padding: 0.8em;
    border-left: 3px solid #546e7a;
    background-color: #fafafa;
  }
  .scholar-link {
    margin-bottom: 1em;
    font-size: 0.95em;
    padding: 0.8em;
    background-color: #f0f0f0;
    border-radius: 3px;
  }
  .scholar-link a {
    font-weight: 600;
    text-decoration: underline;
    color: #34495e;
  }
  .divider {
    margin: 1em 0;
    border-top: 1px solid #ddd;
  }
  .year-heading {
    margin-top: 1.2em;
    margin-bottom: 0.7em;
    font-size: 1.5em;
    color: #333;
  }
</style>

<div class="publications-container">
  {% if site.author.googlescholar %}
    <div class="scholar-link">
      You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.
    </div>
  {% endif %}

  <h2 class="section-heading">Research Articles</h2>
  
  <div class="divider"></div>
  
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
