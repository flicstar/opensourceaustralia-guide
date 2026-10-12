---
layout: category
category: government
title: Government procurement and policy
permalink: /government
research_backlog_anchor: government-procurement-and-policy
---

{% assign entries = site.data.category_data["government"] %}

{% assign group = entries | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}