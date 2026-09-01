---
layout: page
title: "Hobbies, Collectibles & Tech"
permalink: /category/hobbies-tech/
---

# Hobbies, Collectibles & Tech

Model kits, collectibles, audio gear, and cameras genuinely made in Japan.

<ul>
{% assign posts = site.posts | where: "category", "hobbies-tech" %}
{% for post in posts %}
  <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a></li>
{% endfor %}
{% if posts.size == 0 %}
  <li><em>No articles in this category yet — check back soon.</em></li>
{% endif %}
</ul>
