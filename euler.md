---
title: Burning the Midnight Euler
permalink: /euler/
layout: default
---

# Project Euler Problems I’ve Solved

A running list of problems I’ve enjoyed, with explanations and clean solutions.

{% raw %}{% for post in site.posts %}
{% if post.categories contains 'euler' %}
- **[{{ post.title }}]({{ post.url }})** – {{ post.date | date: "%b %d, %Y" }}  
  {{ post.excerpt | strip_html | truncate: 160 }}
{% endif %}
{% endfor %}{% endraw %}

[See all posts →](/)