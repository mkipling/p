---
title: Writing
---

<ul class="index">
{% assign writing = site.w | where_exp: "item", "item.title != 'Writing'" %}
{% for w in writing %}
<li><a href="{{ w.url }}">{{ w.title }}</a></li>
{% endfor %}
</ul>
