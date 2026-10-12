---
layout: category
category: hackerspaces-makerspaces
title: "Hackerspaces and makerspaces"
permalink: /hackerspaces-makerspaces
research_backlog_anchor: hackerspaces-and-makerspaces
---

{% assign entries = site.data.category_data["hackerspaces-makerspaces"] %}

{% assign group = entries | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}
