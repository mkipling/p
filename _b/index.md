---
title: Books
---

<ul class="index">
{% assign books = site.b | where_exp: "item", "item.title != 'Books'" %}
{% for b in books %}
<li><a href="{{ b.url }}">{{ b.title }}</a> by {{ b.author }}</li>
{% endfor %}
</ul>
