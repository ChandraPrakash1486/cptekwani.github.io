---
layout: default
title: My Dev Blog & Portfolio
---

# {{ site.title }}

Welcome! Here are my blog categories:

<ul>
  {% for repo in site.data.repos %}
    <li>
      <a href="{{ repo.html_url }}" target="_blank">{{ repo.name }}</a>
      {% if repo.description %}<br><small>{{ repo.description }}</small>{% endif %}
    </li>
  {% endfor %}
</ul>
