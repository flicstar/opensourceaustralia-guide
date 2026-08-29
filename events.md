---
layout: event
title: "Events"
permalink: /events
description: "Conferences, meetups and community events for open source in Australia."
---

{% assign events = site.data.events %}

<div class="category-summary">Australia has open source events ranging from national conferences to free monthly meetups. Check the organiser's site for current information.</div>

<span>{% include icons/construction.svg %}</span> Checkout my [Research backlog](https://github.com/flicstar/opensourceaustralia-guide/blob/main/RESEARCH-BACKLOG.md#events){:target="_blank"} file to see what I've captured so far, and let me know what I've missed. {% include icons/construction.svg %}

## Conferences

{% assign group = events | where: "type", "conferences" | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}

## Regular gatherings and meetups

{% assign group = events | where: "type", "regular-gatherings" | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}

## Hackathons

{% assign group = events | where: "type", "hackathons" | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}

## Community celebration days

{% assign group = events | where: "type", "community-celebration-days" | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}
