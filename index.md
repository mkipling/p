---
title: "Index"
---

### Other

- [Article 1](/article1)

### [p](/p)
{% for p in site.p %}
  <a href="{{ p.url }}">{{ p.title }} by {{ p.author }}</a><br>
{% endfor %}

### [r](/r)
{% for r in site.r %}
  <a href="{{ r.url }}">{{ r.title }}</a><br>
{% endfor %}
