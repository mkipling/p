---
title: Articles
---

<ul class="index">
{% assign articles = site.a | where_exp: "item", "item.title != 'Articles'" %}
{% for a in articles %}
<li><a href="{{ a.url }}">{{ a.title }}</a></li>
{% endfor %}
</ul>
