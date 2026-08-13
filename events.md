---
layout: page
title: "Events"
permalink: /events
description: "Conferences, meetups and community events for open source in Australia."
---

{% assign events = site.data.events %}

Open source events in Australia: conferences, meetups, hackathons and community gatherings.

Checkout my [Research backlog](https://github.com/flicstar/opensourceaustralia-guide/blob/main/RESEARCH-BACKLOG.md){:target="_blank"} file to see what I've captured so far, and let me know what I've missed.

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

Section blurb.

{% assign group = events | where: "type", "hackathons" | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}

## Community celebration days

{% assign group = events | where: "type", "community-celebration-days" | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}