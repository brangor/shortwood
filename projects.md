---
layout: page
title: Projects
permalink: /projects/
---
Shortwood {{ page.title }}

{{ for project in site.projects }}
  <h2>{{ project.title }}</h2>
  <p> {{ project.description }} </p>
  {% if !project.award.nil? %}
  <h3> {{ Awards | pluralize(project.award.count) }} </h3>
  <ul>
    {% project.award.each do |award| %}
    <li> {{ award }} </li>
    {% endeach %}
  </ul>
  {% endif %}
  <p> {{ project.content | markdownify }} </p>
{{ endfor }}
