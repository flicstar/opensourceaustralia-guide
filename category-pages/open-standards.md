---
layout: category
category: open-standards
title: Open standards
permalink: /open-standards
---

{% assign entries = site.data.category_data["open-standards"] %}

<span>{% include icons/construction.svg %}</span> Checkout my [Research backlog](https://github.com/flicstar/opensourceaustralia-guide/blob/main/RESEARCH-BACKLOG.md){:target="_blank"} file to see what I've captured so far, and let me know what I've missed. {% include icons/construction.svg %}

{% assign group = entries | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}