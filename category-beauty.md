---
layout: page
title: "Beauty & Personal Care"
permalink: /category/beauty/
---

# Beauty & Personal Care (J-Beauty)

Skincare, hair care, and body care genuinely made in Japan.

<ul>
{% assign posts = site.posts | where: "category", "beauty" %}
{% for post in posts %}
  <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a></li>
{% endfor %}
{% if posts.size == 0 %}
  <li><em>No articles in this category yet — check back soon.</em></li>
{% endif %}
</ul>
