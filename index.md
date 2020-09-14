---
title: "Index"
---

[Recipes](/r)

### Other

- [Article 1](/article1)

### P
{% for p in site.p %}
  <a href="{{ p.url }}">{{ p.title }}</a><br>
{% endfor %}

### Tests

{% for test in site.tests %}
  <a href="{{ test.url }}">{{ test.Title }}</a><br>
{% endfor %}
