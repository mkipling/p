
<h3>Recipes</h3>

<ul class="index">
{% assign recipes = site.r | where_exp: "item", "item.title != 'Recipes'" %}
{% for r in recipes %}
  <li><a href="{{ r.url }}">{{ r.title }}</li>
{% endfor %}
</ul>
