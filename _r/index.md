---
title: "Recipes"
---

{% for r in site.r %}
  <a href="{{ r.url }}">{{ r.title }}</a><br>
{% endfor %}
