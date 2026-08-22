---
layout: category
category: open-source-hardware
title: Open Source Hardware
permalink: /open-source-hardware
---

{% assign entries = site.data.category_data["open-source-hardware"] %}

Intro prose goes here.

{% assign group = entries | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}