---
layout: category
category: organisations
title: "Organisations and Groups"
permalink: /organisations
---

{% assign entries = site.data.category_data["organisations"] %}

Intro prose goes here.

{% assign group = entries | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}