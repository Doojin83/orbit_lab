---
layout: default
title: "HOME"
nav_order: 1
---

<p align="center">
  <img src="/orbit_lab/assets/img/orbit1.jpg" alt="ORBIT LAB Home Banner" width="100%" style="box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);" /><br>
</p>

<p align="center">
  <span style="font-size: 24px; font-weight: bold;">
Welcome to
    <br>
    <span style="font-size: 36px; color: red">ORBIT</span>
    <br>
    (<span style="font-weight: bold; color: red">O</span>ne-chip <span style="font-weight: bold; color: red">R</span>ealization of <span style="font-weight: bold; color: red">B</span>oundless <span style="font-weight: bold; color: red">I</span>ntegrated <span style="font-weight: bold; color: red">T</span>echnology)
    <br>
    LAB!</span><br>
    <br>
  <span style="font-size: 16px; color: red">
If you're an undergraduate or future graduate student eager to explore research with ORBIT LAB, feel free to contact us anytime.
  </span>
</p>

## 📰 Latest News

{% for year in site.data.news %}
  {% assign year_items = year[1] %}
  {% for item in year_items %}
  - <strong>{{ item.date }}</strong>: {{ item.title }}
  {% endfor %}
{% endfor %}
