---
layout: category
category: open-science
title: Open Science
permalink: /open-science

{% assign entries = site.data.category_data["open-science"] %}

Intro prose goes here.

{% assign group = entries | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}