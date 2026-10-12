---
layout: category
category: open-standards
title: Open standards
permalink: /open-standards
research_backlog_anchor: open-standards
---

{% assign entries = site.data.category_data["open-standards"] %}

{% assign group = entries | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}