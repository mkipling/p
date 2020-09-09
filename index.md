---
title: "Index"
---

[Recipes](/r)

### Other

- [Article 1](/article1)

### Tests

{% for test in site.tests %}
  <a href="{{ test.url }}">{{ test.Title }}</a><br>
{% endfor %}
