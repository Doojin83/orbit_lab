<h2>ORBIT LAB News</h2>

{% for year in site.data.news %}
<details>
  <summary><strong>{{ year[0] }}</strong></summary>
  <ul>
    {% for item in year[1] %}
    <li><strong>{{ item.date }}</strong> {{ item.title }}</li>
    {% endfor %}
  </ul>
</details>
{% endfor %}
