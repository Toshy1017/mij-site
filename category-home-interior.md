---
layout: page
title: "Home, Interior & Crafts"
permalink: /category/home-interior/
---

# Home, Interior & Crafts

Interior goods, traditional crafts, and lifestyle items genuinely made in Japan.

<ul>
{% assign posts = site.posts | where: "category", "home-interior" %}
{% for post in posts %}
  <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a></li>
{% endfor %}
{% if posts.size == 0 %}
  <li><em>No articles in this category yet — check back soon.</em></li>
{% endif %}
</ul>
