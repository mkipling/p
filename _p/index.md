---
title: Poems
---

{% for p in site.p %}
  {% if p.title != "Poems" %}
    [{{p.title}}]({{p.url}}) by {{p.author}}
  {% endif %}
{% endfor %}
