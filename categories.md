---
title: Portfolio
permalink: /portfolio/
---
{%- if site.categories.size > 0 -%}
<div>
  {% for category in site.categories %}
    {% include product-card.html title=category.title
                                 image=category.image
                                 description=category.title %}
  {% endfor %}
</div>
{%- else -%}
<h2> There are currently no categories </h2>
{%- endif -%}
