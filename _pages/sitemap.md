---
layout: archive
title: "Sitemap"
title_zh: "站点地图"
permalink: /sitemap/
author_profile: true
---

{% include base_path %}

<span class="lang-en">A list of all the posts and pages found on the site. For you robots out there is an [XML version]({{ base_path }}/sitemap.xml) available for digesting as well.</span><span class="lang-zh">本站所有文章与页面的列表。另有供爬虫使用的 [XML 版本]({{ base_path }}/sitemap.xml)。</span>

<h2><span class="lang-en">Pages</span><span class="lang-zh">页面</span></h2>
{% for post in site.pages %}
  {% include archive-single.html %}
{% endfor %}

<h2><span class="lang-en">Posts</span><span class="lang-zh">文章</span></h2>
{% for post in site.posts %}
  {% include archive-single.html %}
{% endfor %}

{% capture written_label %}'None'{% endcapture %}

{% for collection in site.collections %}
{% unless collection.output == false or collection.label == "posts" %}
  {% capture label %}{{ collection.label }}{% endcapture %}
  {% if label != written_label %}
  <h2>{{ label }}</h2>
  {% capture written_label %}{{ label }}{% endcapture %}
  {% endif %}
{% endunless %}
{% for post in collection.docs %}
  {% unless collection.output == false or collection.label == "posts" %}
  {% include archive-single.html %}
  {% endunless %}
{% endfor %}
{% endfor %}
