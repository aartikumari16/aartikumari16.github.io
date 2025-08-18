---
layout: home
title: "Home"
author_profile: true
permalink: /
---


# Welcome to My Portfolio 🎉

I’m **Aarti Kumari**, an AI & Machine Learning enthusiast passionate about transforming data into real-world solutions.  
Here’s a selection of my projects, articles, and experiments.  

[Work with Me](https://www.fiverr.com/aartikumari16){: .btn .btn--primary}

---

<h2>🚀 Featured Projects</h2>
<ul>
  {% assign apps_page = site.pages | where: "projects", true | first %}
  {% if apps_page %}
    {{ apps_page.content }}
  {% endif %}
</ul>

