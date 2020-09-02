---
layout: page
title: About Us
permalink: /about/
published: false
---
## We're Shortwood Creative

### Here's who we be

{% for staff_member in site.staff_members %}
  <h4>{{ staff_member.name }} - {{ staff_member.position }}</h4>
  <p>{{ staff_member.content | markdownify }}</p>
{% endfor %}
