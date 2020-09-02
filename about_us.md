---
title: About Us
permalink: /about/
published: true
---
## We're Shortwood Creative

### Here's who we be

{% for staff_member in site.staff_members %}
  <h4><a href="{{ staff_member.url }}">{{ staff_member.name }}</a> - {{ staff_member.position }}</h4>
  <p>{{ staff_member.excerpt | markdownify }}</p>
{% endfor %}
