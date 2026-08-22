---
layout: category
category: government
title: Government procurement and policy
permalink: /government
---

{% assign entries = site.data.category_data["government"] %}

Intro prose goes here.

{% assign group = entries | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}