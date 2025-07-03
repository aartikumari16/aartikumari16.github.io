---
layout: single
title: "Projects"
permalink: /projects/
author_profile: true
---

Here are a few highlighted projects.

---

<ul>
{% for p in site.data.projects %}
  <li style="margin-bottom:1rem;">
    <strong><a href="{{ p.url }}">{{ p.name }}</a></strong><br/>
    {{ p.desc }}
    {% if p.live %}
      • <a href="{{ p.live }}">Live Demo</a>
    {% endif %}
    {% if p.stars %}
      {% assign repo = site.github.public_repositories | where: "html_url", p.url | first %}
      • ⭐ {{ repo.stargazers_count }}
    {% endif %}
  </li>
{% endfor %}
</ul>
