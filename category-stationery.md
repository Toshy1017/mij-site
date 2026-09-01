---
layout: page
title: "Stationery & Crafts"
permalink: /category/stationery/
---

# Stationery & Crafts

Pens, notebooks, paper goods, and craft tools genuinely made in Japan.

<ul>
{% assign posts = site.posts | where: "category", "stationery" %}
{% for post in posts %}
  <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a></li>
{% endfor %}
{% if posts.size == 0 %}
  <li><em>No articles in this category yet — check back soon.</em></li>
{% endif %}
</ul>
