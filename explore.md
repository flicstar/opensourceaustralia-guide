---
layout: category
title: Explore
permalink: /explore
---

{% assign categories = site.data.categories %}

## See what's out there

{% assign main = categories | where: "type", "whats-out-there" | sort_natural: "slug" %}
{% for category in main %}
{% assign icon_path = "icons/" | append: category.icon | append: ".svg" %}
<h3 class="explore-heading">
  {% include {{ icon_path }} %}
  <a href="/{{ category.slug }}">{{ category.title }}</a>
</h3>

<p>{{ category.description }}</p>
{% endfor %}

## Find your people

{% assign people = categories | where: "type", "find-your-people" | sort_natural: "slug" %}
{% for category in people %}
{% assign icon_path = "icons/" | append: category.icon | append: ".svg" %}
<h3 class="explore-heading">
  {% include {{ icon_path }} %}
  <a href="/{{ category.slug }}">{{ category.title }}</a>
</h3>

<p>{{ category.description }}</p>
{% endfor %}