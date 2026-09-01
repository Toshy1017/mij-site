---
layout: page
title: "Apparel & Textiles"
permalink: /category/apparel/
---

# Apparel & Textiles

Japanese denim, workwear, traditional clothing, and accessories genuinely made in Japan.

<ul>
{% assign posts = site.posts | where: "category", "apparel" %}
{% for post in posts %}
  <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a></li>
{% endfor %}
{% if posts.size == 0 %}
  <li><em>No articles in this category yet — check back soon.</em></li>
{% endif %}
</ul>
