---
layout: page
title: Projects
permalink: /projects/
---
Shortwood {{ page.title }}

{% for project in site.projects %}
  <h2>{{ project.title }}</h2>
  <p> {{ project.description }} </p>
  {% unless project.awards.nil? %}
  <h3> {{ project.awards.count.to_s }}  </h3>
  <ul>
    {% for award in project.awards %}
    <li> {{ award }} </li>
    {% endfor %}
  </ul>
  {% endunless %}
  <p> {{ project.content | markdownify }} </p>
{% endfor %}
