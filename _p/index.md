---
title: Poems
highlighter: none
---

{% for p in site.p %}
  <a href="{{ p.url }}">{{ p.title }}</a> by {{p.author}}<br />
{% endfor %}
