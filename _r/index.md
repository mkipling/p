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

---

{% assign recipesByCategory = site.r | group_by_exp: "r", "r.category" %}
{% for cat in recipesByCategory %}
  {{ cat }}
  {% if cat.name == "" %}
    <b>No Category</b>
  {% else %}
    <b>{{ cat.name }}</b>
  {% endif %}
  <ul class="index">
    {% for r in cat.items %}
      <li><a href="{{ r.url }}">{{ r.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}

