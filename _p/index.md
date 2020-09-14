---
title: Poems
---

{% assign poems = site.p | where_exp: "item", "item.title != 'Poems'" %}
{% for p in poems %}
  <a href="{{ p.url }}">{{ p.title }}</a> by {{p.author}}<br />
{% endfor %}
