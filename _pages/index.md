---
layout: home
title: "Home"
author_profile: true
---

# Welcome to My Portfolio 🎉

I’m **Aarti Kumari**, an AI & Machine Learning enthusiast passionate about transforming data into real-world solutions.  
Here’s a selection of my projects, articles, and experiments.  

[Work with Me](https://www.fiverr.com/aartikumari16){: .btn .btn--primary}

---

## 🚀 Featured Projects

### [Brain Tumor Classification](https://github.com/aartikumari16/Brain-Tumor-Classification)
A deep learning project using **TensorFlow**, **Keras**, and **OpenCV** for medical image classification.  
`TensorFlow` `Keras` `OpenCV`

---

## 📝 Recent Posts
{% for post in site.posts limit:2 %}
- [{{ post.title }}]({{ post.url | relative_url }})  
  *{{ post.date | date: "%B %d, %Y" }}* — {{ post.excerpt }}
{% endfor %}
