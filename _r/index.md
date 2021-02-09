---
title: Poems
---

<ul class="index">
{% assign poems = site.p | where_exp: "item", "item.title != 'Poems'" %}
{% for p in poems %}
<li><a href="{{ p.url }}">{{ p.title }}</a> by {{ p.author }}</li>
{% endfor %}
</ul>
