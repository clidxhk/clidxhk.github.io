---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

<div style="padding: 20px; margin: 25px 0; background-color: #e3f2fd; border-radius: 8px; border-left: 5px solid #2196f3;">
<h2 style="color: #1565c0; margin-top: 0;">My Research Articles</h2>

{% if site.author.googlescholar %}
  <p style="color: #1976d2;">You can also find my articles on <a href="{{site.author.googlescholar}}" style="color: #0d47a1; text-decoration: underline; font-weight: bold;">my Google Scholar profile</a>.</p>
{% endif %}

<div style="margin-top: 20px; border-top: 1px dashed #90caf9; padding-top: 20px;">
  {% include base_path %}

  {% for post in site.publications reversed %}
    <div style="padding: 15px; margin: 15px 0; background-color: #f8fdff; border-radius: 5px; border-left: 3px solid #64b5f6;">
      {% include archive-single.html %}
    </div>
  {% endfor %}
</div>
</div>
