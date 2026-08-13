---
layout: category
category: organisations-and-groups
title: "Organisations and Groups"
permalink: /organisations-and-groups
description: "Australian organisations, foundations and community groups working in open source."
---

{% assign entries = site.data.directory["organisations-and-groups"] %}

Intro prose goes here.

{% assign group = entries | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}