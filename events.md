---
layout: event
title: "Events"
permalink: /events
description: "Conferences, meetups and community events for open source in Australia."
---

{% assign events = site.data.events %}

<div class="category-summary">Australia has open source events ranging from national conferences to free monthly meetups. Check the organiser's site for current information.</div>

The peak conference for open source in Australia is [Everything Open](https://opensourceaustralia.guide/events#everything-open) run by [Linux Australia](https://opensourceaustralia.guide/organisations#linux-australia). This community event is volunteer-run, and the clue’s in the name \- the event caters to *everything open*: software, hardware, data, government, science, the GLAM sector, and many other open communities.

Other events are specific to their context or topic. You might find a happening by joining a user group specific to the tool, program or protocol you’re interested in, because they usually gather regularly.

You might also find relevant meetups near you by searching for the term “open source” on event platforms like [meetup.com](https://www.meetup.com/topics/opensource/au/){:target="_blank"} and the [Tech Events website](https://techevents.au/?view=national){:target="_blank"}.

<span>{% include icons/construction.svg %}</span> Update my [Research backlog](https://github.com/flicstar/opensourceaustralia-guide/blob/main/RESEARCH-BACKLOG.md#events){:target="_blank"} to let me know what I've missed. {% include icons/construction.svg %}

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

{% comment %}
## Community celebration days

{% assign group = events | where: "type", "community-celebration-days" | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}
{% endcomment %}