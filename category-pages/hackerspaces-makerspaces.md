---
layout: category
category: hackerspaces-makerspaces
title: "Hackerspaces and makerspaces"
permalink: /hackerspaces-makerspaces
description: Directories and networks for finding Australian hackerspaces and makerspaces, community workshops where people share tools, equipment and skills.
image: /assets/images/category/hackerspaces.png
research_backlog_anchor: hackerspaces-and-makerspaces
---

{% assign entries = site.data.category_data["hackerspaces-makerspaces"] %}

If you want to understand how open source works in practice, a hackerspace is a good place to watch it happen.

A hackerspace is a place where people meet to work on projects together. They tend to choose software and hardware that is open, and they have an ethos of sharing what they learn. Some spaces call themselves makerspaces instead. The names get used more or less interchangeably.

What you find inside varies. Soldering irons and a bank of 3D printers. A laser cutter, sometimes a lathe and a welder, plus a wall of donated parts.

Many spaces run as incorporated associations, funded by member fees and steered by a committee elected each year. But not every space is a membership club. Public libraries across Australia run makerspaces that anyone can walk into, often with 3D printers, vinyl cutters and sewing machines. [The Edge](https://www.slq.qld.gov.au/visit/spaces/edge){:target="_blank"} at the State Library of Queensland is one of the larger ones. Universities run them too, mostly for students and staff.

## Finding a space

{% assign group = entries | where: "type", "directories" | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}

## Networks and communities

{% assign group = entries | where: "type", "networks" | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}