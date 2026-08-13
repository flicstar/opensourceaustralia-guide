---
layout: category
category: open-data
title: "Open Data"
permalink: /open-data
description: "Australian open data: government portals, civic tech, GLAM collections, research and spatial data."
---

{% assign entries = site.data.directory["open-data"] %}

Intro prose goes here.

## Government portals

Section blurb.

{% assign group = entries | where: "type", "government-portals" | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}

## Civic tech

Section blurb.

{% assign group = entries | where: "type", "civic-tech" | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}

## GLAM

Section blurb.

{% assign group = entries | where: "type", "glam" | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}