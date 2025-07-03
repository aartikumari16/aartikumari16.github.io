---
layout: single
title: "Projects"
permalink: /projects/
author_profile: true
---

Here are my public GitHub projects. This list updates automatically.

---

<ul>
{%- assign repos = site.github.public_repositories | sort: "stargazers_count" | reverse -%}
{%- for repo in repos -%}
  {%- unless repo.name == site.github.repository_nwo -%}
    <li style="margin-bottom: 1rem;">
      <strong><a href="{{ repo.html_url }}">{{ repo.name }}</a></strong>  
      <br />
      {{ repo.description }}
      <br />
      ⭐ <strong>{{ repo.stargazers_count }}</strong> &nbsp;•&nbsp;
      {{ repo.language }}
    </li>
  {%- endunless -%}
{%- endfor -%}
</ul>
