---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---
<ul>
{% for category in site.data.categories %}
  <li><a href="/{{ category.slug }}">{{ category.title }}</a> — {{ category.summary }}</li>
{% endfor %}
</ul>