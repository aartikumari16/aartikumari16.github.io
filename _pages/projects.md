---
layout: single
title: "Projects"
permalink: /projects/
author_profile: true
---

Below is an auto‑generated list of my public GitHub repositories.  
*It updates each time I push a new project.*

<ul>
{%- for repo in site.github.public_repositories -%}
  {%- unless repo.name == site.github.repository_nwo %}   {# skip the portfolio repo itself #}
  <li>
    <a href="{{ repo.html_url }}">{{ repo.name }}</a>
    – {{ repo.description }}
    <br/>
    <small>⭐ {{ repo.stargazers_count }} · {{ repo.language }}</small>
  </li>
  {%- endunless -%}
{%- endfor -%}
</ul>
