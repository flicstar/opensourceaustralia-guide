---
layout: category
category: organisations
title: "Organisations and groups"
permalink: /organisations
---

{% assign entries = site.data.category_data["organisations"] %}

<span>{% include icons/construction.svg %}</span> This page is a work in progress. Checkout my [Research backlog](https://github.com/flicstar/opensourceaustralia-guide/blob/main/RESEARCH-BACKLOG.md#organisations-and-groups){:target="_blank"} file to see the organisations I still need to add here. {% include icons/construction.svg %}


## Umbrella and backing bodies

These groups hold money, provide legal standing and back volunteer-run events.

{% assign group = entries | where: "type", "umbrella" | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}

## Infrastructure

Groups that run data portals, observing systems and other facilities you can use.

{% assign group = entries | where: "type", "infrastructure" | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}

## Builders

Groups that make and maintain things for the public to use.

{% assign group = entries | where: "type", "builders" | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}

## Communities and gatherings

Groups that bring people together, in person or online.

{% assign group = entries | where: "type", "communities" | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}

## Open access and open science

Groups working to make research available to everyone. You can find the collections and catalogues they support on the [open science](https://opensourceaustralia.guide/open-science) page.

{% assign group = entries | where: "type", "open-science" | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}

## Advocacy and policy

Groups that make the case for open source, open data, and digital rights.

{% assign group = entries | where: "type", "advocacy" | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}