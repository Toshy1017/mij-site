---
layout: page
title: "Kitchenware & Tableware"
permalink: /category/kitchenware/
---

# Kitchenware & Tableware

Knives, cookware, and tableware genuinely made in Japan — from professional-grade knives to everyday ceramics.

<ul>
{% assign posts = site.posts | where: "category", "kitchenware" %}
{% for post in posts %}
  <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a></li>
{% endfor %}
{% if posts.size == 0 %}
  <li><em>No articles in this category yet — check back soon.</em></li>
{% endif %}
</ul>
