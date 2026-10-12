---
layout: category
category: organisations
title: "Organisations and groups"
permalink: /organisations
description: Peak bodies, foundations, user groups and communities working with open source software, hardware, data and research in Australia
image: /assets/images/category/organisations.png
research_backlog_anchor: organisations-and-groups
---

{% assign entries = site.data.category_data["organisations"] %}

Organisations working in open source in Australia include government agencies, universities, foundations, industry bodies and community groups.

Some are national bodies with staff and budgets. Others are small volunteer groups. They run infrastructure, build tools, back events and shape policy.

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

## Communities and user groups

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
