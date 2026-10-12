---
layout: category
category: open-apis
title: Open APIs
permalink: /open-apis
research_backlog_anchor: open-apis
---

{% assign entries = site.data.category_data["apis"] %}

{% assign group = entries | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}