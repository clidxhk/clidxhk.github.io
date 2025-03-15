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
      <h2><a href="{{ base_path }}{{ post.url }}">{{ post.title }}</a></h2>
      <p>{{ post.authors }}</p>
      <p><em>{{ post.venue }}</em>, {{ post.date | default: "1900-01-01" | date: "%Y" }}</p>
      
      {% if post.excerpt and site.read_more != 'enabled' %}
        <p>{{ post.excerpt | markdownify }}</p>
      {% elsif post.excerpt and site.read_more == 'enabled' %}
        <p>{{ post.excerpt | markdownify }} <a href="{{ base_path }}{{ post.url }}" rel="permalink">Read more</a></p>
      {% endif %}
      
      {% if post.citation and post.paperurl %}
        <p>Recommended citation: {{ post.citation }} <a href="{{ post.paperurl }}"><i class="fas fa-fw fa-file-pdf" aria-hidden="true"></i> PDF</a></p>
      {% elsif post.citation %}
        <p>Recommended citation: {{ post.citation }}</p>
      {% elsif post.paperurl %}
        <p><a href="{{ post.paperurl }}"><i class="fas fa-fw fa-file-pdf" aria-hidden="true"></i> Download PDF</a></p>
      {% endif %}
    </div>
  {% endfor %}
{% endfor %}
