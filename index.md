---
layout: default
title: "HOME"
nav_order: 1
---

<p align="center">
  <img src="/orbit_lab/assets/img/home_banner.png" alt="ORBIT LAB Home Banner" width="80%">
</p>

Welcome to the **ORBIT LAB**  
(One-chip Realization of Boundless Integrated Technology)  
led by **Prof. Doojin Jang** at Cheongju University.

## 📰 Latest News

{% assign all_news = site.data.news | sort_natural: 'first' | reverse %}
{% for year in all_news limit: 1 %}
  {% for item in year[1] limit: 3 %}
  - <strong>{{ item.date }}</strong>: {{ item.title }}
  {% endfor %}
{% endfor %}

[👉 View all news]({{ '/pages/news.md' | relative_url }})
