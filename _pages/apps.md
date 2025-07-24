---
layout: page
title: My Apps
permalink: /apps/
---

<style>
.app-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 1.5rem;
  padding: 1rem 0;
}
.app-card {
  border: 1px solid #ddd;
  border-radius: 12px;
  padding: 1rem;
  box-shadow: 0 4px 6px rgba(0,0,0,0.05);
  transition: all 0.3s ease;
  background: white;
}
.app-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 8px 16px rgba(0,0,0,0.1);
}
.app-title {
  font-size: 1.2rem;
  font-weight: bold;
  color: #2b2b2b;
}
.app-desc {
  margin: 0.5rem 0;
  font-size: 0.95rem;
  color: #555;
}
.app-link {
  display: inline-block;
  margin-top: 0.5rem;
  padding: 0.4rem 0.8rem;
  background: #007acc;
  color: white;
  border-radius: 8px;
  text-decoration: none;
}
.app-link:hover {
  background: #005f99;
}
</style>

## 🚀 Featured Apps

<div class="app-grid">

<div class="app-card">
  <div class="app-title">Auto EDA Dashboard</div>
  <div class="app-desc">Upload a CSV and get automatic data profiling, visualizations, and insights.</div>
  <a class="app-link" href="https://aarti-eda-dashboard.streamlit.app" target="_blank">Launch App</a>
</div>

</div>
