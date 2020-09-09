---
title: "Recipes"
---

- [Red Lentil Dahl](/r/red-lentil-dahl-1)
- [Sour Dough Starter](/r/sourdough-starter)

List:

{% for item in site.recipes.articles %}
  {{ item.title }}
{% endfor %}
