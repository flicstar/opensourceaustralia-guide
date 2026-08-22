---
layout: category
category: organisations-and-groups
title: "Organisations and Groups"
permalink: /organisations-and-groups
---

{% assign entries = site.data.category_data["organisations-and-groups"] %}

Intro prose goes here.

{% assign group = entries | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}