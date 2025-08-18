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

---

{% for section in site.data.features %}
  <h2>{{ section.title }}</h2>
  <div class="feature-cards">
    {% for item in section.items %}
      <div class="card">
        <h3><a href="{{ item.url }}">{{ item.title }}</a></h3>
        <p>{{ item.description }}</p>
        <a href="{{ item.url }}" class="btn">{{ item.btn_label }}</a>
      </div>
    {% endfor %}
  </div>
{% endfor %}
