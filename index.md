---
layout: default
title: "HOME"
nav_order: 1
---

<p align="center">
  <img src="/orbit_lab/assets/img/home_banner.png" alt="ORBIT LAB Home Banner" width="80%">
</p>

<p align="center">
  <span style="font-size: 20px; color: blue; font-weight: bold;">
Welcome to the **ORBIT LAB**  
  </span>
</p>

## 📰 Latest News

{% for year in site.data.news %}
  {% assign year_items = year[1] %}
  {% for item in year_items %}
  - <strong>{{ item.date }}</strong>: {{ item.title }}
  {% endfor %}
{% endfor %}
