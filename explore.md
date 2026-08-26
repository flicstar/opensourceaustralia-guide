---
layout: page
title: Explore
permalink: /explore
---

{% assign categories = site.data.categories %}
{% for category in categories %}
{% assign icon_path = "icons/" | append: category.icon | append: ".svg" %}
<h2 class="explore-heading">
  {% include {{ icon_path }} %}
  <a href="/{{ category.slug }}">{{ category.title }}</a>
</h2>

<p>{{ category.description }}</p>
{% endfor %}