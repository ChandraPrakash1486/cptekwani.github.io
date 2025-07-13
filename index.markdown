---
layout: home
title: My Dev Blog & Portfolio
---

<div class="hero-section">
  <h1 class="hero-title">{{ site.title }}</h1>
  <p class="hero-subtitle">{{ site.description }}</p>
</div>

Welcome! Here are my blog categories:

<ul>
  {% for repo in site.data.repos %}
    <li>
      <a href="{{ repo.html_url }}" target="_blank">{{ repo.name }}</a>
      {% if repo.description %}<br><small>{{ repo.description }}</small>{% endif %}
    </li>
  {% endfor %}
</ul>
