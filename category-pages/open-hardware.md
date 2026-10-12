---
layout: category
category: open-source-hardware
title: Open source hardware
permalink: /open-source-hardware
research_backlog_anchor: open-hardware
---

{% assign entries = site.data.category_data["open-source-hardware"] %}

{% assign group = entries | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}