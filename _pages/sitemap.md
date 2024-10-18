---
layout: archive
title: "Sitemap"
permalink: /sitemap/
author_profile: true
---

{% include base_path %}



<h2>Blog Posts</h2>
{% for post in site.posts %}
  {% include archive-single.html %}
{% endfor %}

<h2>Portfolio</h2>
{% for item in site.portfolio %}
  {% include archive-single.html %}
{% endfor %}
