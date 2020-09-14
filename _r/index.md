---
title: "Recipes"
---

{% for r in site.r %}
  <a href="{{ r.url }}">{{ r.Title }}</a><br>
{% endfor %}
