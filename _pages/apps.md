---
layout: single
title: "My Apps"
permalink: /apps/
projects: true
author_profile: true
---

Below are some of the apps I’ve built using Streamlit and Machine Learning. Click to explore!

<style>
.app-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
  gap: 20px;
  margin-top: 30px;
}
.app-card {
  border: 1px solid #ccc;
  border-radius: 12px;
  padding: 15px;
  text-align: center;
  box-shadow: 0 4px 8px rgba(0,0,0,0.05);
  transition: transform 0.2s;
}
.app-card:hover {
  transform: translateY(-5px);
}
.app-card img {
  width: 100%;
  height: 150px;
  object-fit: cover;
  border-radius: 8px;
}
.app-card h3 {
  margin: 10px 0 5px;
}
.app-card p {
  font-size: 0.9rem;
  color: #555;
}
.app-card a {
  display: inline-block;
  margin-top: 10px;
  padding: 8px 16px;
  background: #007ACC;
  color: white;
  border-radius: 5px;
  text-decoration: none;
}
</style>

<div class="app-grid">

  <div class="app-card">
    <img src="/assets/images/eda.png" alt="Auto EDA App">
    <h3>Auto EDA Tool</h3>
    <p>Upload your dataset and get a full exploratory analysis.</p>
    <a href="https://auto-eda-app.streamlit.app/" target="_blank">View App</a>
  </div>

  <div class="app-card">
    <img src="/assets/images/brain-mri.jpg" alt="Brain MRI Image Classifier">
    <h3>Brain MRI Image Classifier</h3>
    <p>Upload a Brain MRI Image and get it classified according to Tumour Type.</p>
    <a href="https://huggingface.co/spaces/aartikumari16/mri-brain-tumour-image-classifier" target="_blank">View App</a>
  </div>


</div>
