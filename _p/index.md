---
title: Poems
---

{% for p in site.p %}
  {% if p.title != "Poems" %}
    <a href="{{ p.url }}">{{ p.title }}</a><br>
  {% endif %}
{% endfor %}
