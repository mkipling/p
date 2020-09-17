---
title: "Recipes"
---

{% assign recipes = site.r | where_exp: "item", "item.title != 'Recipes'" %}
{% for r in recipes %}
1. <a href="{{ r.url }}">{{ r.title }}
{% endfor %}
