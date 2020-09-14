---
title: "Recipes"
---

{% assign recipes = site.r | where_exp: "item", "item.title != 'Recipes'" %}
{% for r in recipes %}
  <a href="{{ r.url }}">{{ r.title }}</a> <br />
{% endfor %}
