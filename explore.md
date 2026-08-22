---
layout: page
title: Explore
permalink: /explore
---

{% for category in site.data.categories %}
### [{{ category.title }}]({{ category.slug | prepend: "/" }})

{{ category.description }}
{% endfor %}