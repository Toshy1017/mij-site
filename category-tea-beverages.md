---
layout: page
title: "Tea, Beverages & Spirits"
permalink: /category/tea-beverages/
---

# Tea, Beverages & Spirits

Matcha, green tea, whisky, sake, and more — genuinely Japan-made drinks worth seeking out.

<ul>
{% assign posts = site.posts | where: "category", "tea-beverages" %}
{% for post in posts %}
  <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a></li>
{% endfor %}
{% if posts.size == 0 %}
  <li><em>No articles in this category yet — check back soon.</em></li>
{% endif %}
</ul>
