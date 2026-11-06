---
layout: page
title: Explore
permalink: /explore
---

## What's out there

{% assign categories = site.data.categories %}
{% for category in categories %}
{% assign icon_path = "icons/" | append: category.icon | append: ".svg" %}
<h2 class="explore-heading">
  {% include {{ icon_path }} %}
  <a href="/{{ category.slug }}">{{ category.title }}</a>
</h2>

<p>{{ category.description }}</p>
{% endfor %}

&nbsp;

## Find your people

<h2 class="explore-heading">
  <a href="/chat">Community chat</a>
</h2>

<p>Online spaces where people talk about all things open.</p>

<h2 class="explore-heading">
  <a href="/follow">Recommended follows </a>
</h2>

<p>Podcasts, videos and books from Australian hosts, guests and authors.</p>