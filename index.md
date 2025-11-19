---
# No title here on purpose → browser tab uses the site.title from _config.yml
# If you WANT a different front-matter title, add: title: "Custom Home Title"
permalink: /home/
layout: default
---

<div style="text-align:center; padding:5rem 1rem;">
  <h1>Hi, I’m Zak Boston</h1>
  <p style="font-size:1.3rem; opacity:0.9;">
    I solve project euler problems and post about clean solutions.
  </p>
  <p>
    <a href="/euler" style="font-size:1.2rem; padding:0.8rem 1.5rem; background:#58a6ff; color:black; border-radius:8px; text-decoration:none;">
      See All Code Solutions →
    </a>
  </p>
</div>

## Recent Solutions

{% for post in site.posts limit:6 %}
<!-- your beautiful preview loop from before -->
{% endfor %}

<div style="text-align:center; margin-top:4rem;">
  <a href="/euler">View all {{ site.posts.size }} solutions →</a>
</div>