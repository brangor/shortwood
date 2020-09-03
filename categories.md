---
title: Categories
permalink: /categories/
---
<div>
  {% for category in site.data.categories %}
    <a href="{{ category.link }}"> {{- category.title -}} </a>
  {% endfor %}
</div>
