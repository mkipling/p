---
title: Recipes
---

{% assign recipesByCategory = site.r | group_by_exp: "r", "r.category" %}
{% for cat in recipesByCategory %}

  {% if cat.name == nil %}Not Categorized{% else %}{{ cat.name }}{% endif %}

  <ul class="index">
    {% for r in cat.items %}
      <li><a href="{{ r.url }}">{{ r.title }}</a></li>
    {% endfor %}
  </ul>
  
{% endfor %}

