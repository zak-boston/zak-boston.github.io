---
layout: default
title: Home
---

<div class="home-header" style="text-align: center; padding: 4rem 1rem; margin-bottom: 3rem;">
  <h1>Hi, I’m {{ site.author | default: "Zak Boston" }}</h1>
  <p style="font-size: 1.3rem; opacity: 0.9;">
    Data Scientist • First Principles Thinker • Forever Curious
  </p>
  <p>
    <a href="/euler" class="btn">View All Code Problems →</a>
  </p>
</div>

## Latest Solutions

{% for post in site.posts limit:6 %}
  <article class="post-preview" style="margin-bottom: 2.5rem; padding-bottom: 1.5rem; border-bottom: 1px solid rgba(255,255,255,0.1);">
    <h2 style="margin-bottom: 0.4rem;">
      <a href="{{ post.url }}" style="color: #58a6ff;">{{ post.title }}</a>
    </h2>

    <div style="margin-bottom: 0.8rem; opacity: 0.8; font-size: 0.95rem;">
      {{ post.date | date: "%B %d, %Y" }}
      {% if post.categories contains 'euler' %} 
        — Project Euler
      {% endif %}
    </div>

    <p style="margin-top: 0.5rem;">
      {{ post.excerpt | strip_html | truncate: 220 }}
    </p>

    <div>
      <a href="{{ post.url }}" style="color: #58a6ff; font-weight: 600;">Read full solution →</a>
    </div>
  </article>
{% endfor %}

<div style="text-align: center; margin-top: 3rem;">
  <a href="/euler" style="font-size: 1.2rem; color: #58a6ff;">
    See all {{ site.posts.size }} solutions →
  </a>
</div>