---
title: Poems
---

{% for p in site.p %}
  {% if p.title != "Poems" %}
    <a markdown = "0" href="{{ p.url }}">{{ p.title }}</a> by {{p.author}}<br />
  {% endif %}
{% endfor %}
