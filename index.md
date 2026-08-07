---
layout: home
---

<img src="{{ '/assets/images/under-construction.svg' }}"
     alt="" width="200" height="147" class="construction-sign">

## Under construction

This site is new and still filling out. Expect gaps.

If you know something that belongs here, [tell me](/about).

### Working in the open

I am writing about the build as I go. I feel exposed but it may end up a higher quality product that way. Follow along over on [my blog](https://flicstar.com).

<ul>
{% for category in site.data.categories %}
  <li><a href="/{{ category.slug }}">{{ category.title }}</a> — {{ category.summary }}</li>
{% endfor %}
</ul>