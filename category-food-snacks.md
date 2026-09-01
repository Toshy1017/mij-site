---
layout: page
title: "Snacks, Food & Seasonings"
permalink: /category/food-snacks/
---

# Snacks, Food & Seasonings

Japanese snacks, staples, and seasonings genuinely made in Japan.

<ul>
{% assign posts = site.posts | where: "category", "food-snacks" %}
{% for post in posts %}
  <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a></li>
{% endfor %}
{% if posts.size == 0 %}
  <li><em>No articles in this category yet — check back soon.</em></li>
{% endif %}
</ul>
