---
title: "Recipes"
---

<ul>
{% assign recipes = site.r | where_exp: "item", "item.title != 'Recipes'" %}
{% for r in recipes %}
  <li><a href="{{ r.url }}">{{ r.title }}</a></li>
{% endfor %}
</ul>
