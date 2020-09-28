---
title: Recipes
---

<ul class="index">
{% assign recipes = site.r | where_exp: "item", "item.title != 'Recipes'" | sort: "category" %}
{% for r in recipes %}
  
  {% assign currentCategory = r.category %}
  {% if currentCategory != category %}
    <b>Category: {{ r.category }}</b>
    {% assign category = currentdate %} 
  {% endif %}
  
  <li><a href="{{ r.url }}">{{ r.title }}</a></li>
{% endfor %}
</ul>
