---
layout: category
category: follow
title: "Recommended follows"
permalink: /follow
description: Books, podcasts, videos and people worth following, from Australian hosts, guests and authors.
image: /assets/images/category/follow.png
issue_template: add-entry.yml
---

{% assign entries = site.data["follow"] %}

Books, podcasts, and videos with an Australian connection. Add your favourites here.

## Books

{% assign group = entries | where: "type", "books" | sort_natural: "name" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}

## Newsletters

{% assign group = entries | where: "type", "newsletters" | sort_natural: "name" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}

## Podcasts

{% assign group = entries | where: "type", "podcasts" | sort_natural: "name" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}

## Videos

Sessions from [Everything Open](/events#everything-open) conferences are available to watch on the [Everything Open YouTube channel](https://www.youtube.com/@EverythingOpen).

{% assign group = entries | where: "type", "videos" | sort_natural: "name" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}