---
title: Recipes
---

<ul class="index">
{% assign recipes = site.r | where_exp: "item", "item.title != 'Recipes'" | sort: "category" %}
{% for r in recipes %}
  <li><a href="{{ r.url }}">{{ r.title }}</a></li>
{% endfor %}
</ul>

---

{% assign recipesByCategory = site.r | group_by_exp: "r", "r.category" %}
{% for cat in recipesByCategory %}
{% if cat.name == nil %}
No Category
{% else %}
{{ cat.name }}
{% endif %}
<ul class="index">
{% for r in cat.items %}
<li><a href="{{ r.url }}">{{ r.title }}</a></li>
{% endfor %}
</ul>
{% endfor %}

