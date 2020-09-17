---
title: Articles
---

{% assign articles = site.a | where_exp: "item", "item.title != 'Articles'" %}
{% for a in articles %}
  <a href="{{ a.url }}">{{ a.title }}</a><br />
{% endfor %}
