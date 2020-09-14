---
title: "Index"
---

### Other

- [Article 1](/article1)

### [poems](/p)
{% for p in site.p %}
  <a href="{{ p.url }}">{{ p.title }}</a> by {{ p.author }}<br>
{% endfor %}

### [recipes](/r)
{% for r in site.r %}
  <a href="{{ r.url }}">{{ r.title }}</a><br>
{% endfor %}
