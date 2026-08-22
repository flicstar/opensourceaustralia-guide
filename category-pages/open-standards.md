---
layout: category
category: open-standards
title: Open Standards
permalink: /open-standards
---

{% assign entries = site.data.category_data["open-standards"] %}

Intro prose goes here.

{% assign group = entries | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}