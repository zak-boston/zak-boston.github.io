---
---                  # ← Required for Liquid to work with remote_theme
layout: default
---

<div style="text-align:center; padding:6rem 1rem; background:linear-gradient(135deg, #1a1a2e, #16213e); margin:-2rem -2rem 4rem -2rem;">
  <h1 style="font-size:3.8rem; margin-bottom:0.5rem;">Zak Boston</h1>
  <p style="font-size:1.5rem; opacity:0.9; margin:1rem 0;">
    Solving Project Euler problems • One clean solution at a time
  </p>
  <p style="margin-top:2rem;">
    <a href="/euler" style="font-size:1.3rem; padding:1rem 2rem; background:#58a6ff; color:#000; font-weight:600; border-radius:12px; text-decoration:none; box-shadow:0 4px 15px rgba(88,166,255,0.4);">
      Browse All Euler Solutions →
    </a>
  </p>
</div>

## Recent Solutions

{% for post in site.posts limit:5 %}
<article style="background:rgba(255,255,255,0.03); padding:2rem; margin:2.5rem 0; border-radius:12px; border-left:4px solid #58a6ff; transition:all 0.3s;">
  <h2 style="margin:0 0 0.5rem 0; font-size:1.8rem;">
    <a href="{{ post.url }}" style="color:#58a6ff; text-decoration:none;">{{ post.title }}</a>
  </h2>

  <div style="opacity:0.8; margin-bottom:1rem; font-size:0.95rem;">
    {{ post.date | date: "%B %d, %Y" }}
    {% if post.problem_number %} • Problem {{ post.problem_number }}{% endif %}
  </div>

  <p style="line-height:1.7; margin:1rem 0;">
    {{ post.excerpt | strip_html | truncate: 240 }}
  </p>

  <div>
    {% if post.tags %}
      {% for tag in post.tags %}
        {% if tag == 'easy' %}<span class="tag tag-easy">Easy</span>{% endif %}
        {% if tag == 'medium' %}<span class="tag tag-medium">Medium</span>{% endif %}
        {% if tag == 'hard' %}<span class="tag tag-hard">Hard</span>{% endif %}
        {% if tag == 'python' %}<span class="tag tag-python">Python</span>{% endif %}
        {% if tag == 'math' %}<span class="tag tag-dp">Math</span>{% endif %}
        {% if tag == 'number-theory' %}<span class="tag tag-one-pass">Number Theory</span>{% endif %}
        {% if tag != 'easy' and tag != 'medium' and tag != 'hard' and tag != 'python' and tag != 'math' and tag != 'number-theory' %}
          <span class="tag" style="background:#6f42c1;">{{ tag }}</span>
        {% endif %}
      {% endfor %}
    {% endif %}

    <a href="{{ post.url }}" style="float:right; color:#58a6ff; font-weight:600; text-decoration:none;">
      Read solution →
    </a>
  </div>
</article>
{% endfor %}

<div style="text-align:center; margin:4rem 0;">
  <a href="/euler" style="font-size:1.3rem; color:#58a6ff;">
    View all {{ site.posts.size }} Project Euler solutions →
  </a>
</div>