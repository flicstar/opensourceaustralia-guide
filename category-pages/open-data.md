---
layout: category
category: open-data
title: "Open data"
permalink: /open-data
---

{% assign entries = site.data.category_data["open-data"] %}

Open data is information that anyone can access, use and share, released under a licence that says so.

You might be surprised by how much Australian data is freely available to you. To work with open data, you can download it as a file or you can use an API, which gives you the data as it changes.

There's no single place all of it lives. Publishing is split across federal agencies, state and territory governments, universities, research bodies and volunteer-run community projects.

## Government portals

Australian Government agencies are expected to make their non-sensitive data open by default. Every level of government publishes data, and each runs its own catalogue. The federal catalogue aggregates some state and local material, but not all of it, so it's worth checking your state portal directly.

{% assign group = entries | where: "type", "government-portals" | sort_natural: "sort_key" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry show_run_by=false %}
{% endfor %}

## Civic tech

Civic tech projects take government information that that anyone can see but few can use, and republish it in a form people can actually work with.

{% assign group = entries | where: "type", "civic-tech" | sort_natural: "sort_key" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry show_run_by=false %}
{% endfor %}

## GLAM

GLAM stands for Galleries, Libraries, Archives and Museums. Open GLAM is a movement for free and open access to digital cultural heritage: the collections, catalogues and digitised material that these institutions hold.

{% assign group = entries | where: "type", "glam" | sort_natural: "sort_key" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry show_run_by=false %}
{% endfor %}

## Transport

Timetables, stop locations, real-time vehicle positions and road network data. Most Australian transport agencies publish in GTFS, an open standard for transit data.

{% assign group = entries | where: "type", "transport" | sort_natural: "sort_key" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry show_run_by=false %}
{% endfor %}

## Geospatial and mapping

Spatial data is any information with a location attached to it, describing where something is and what shape and size it takes. You use geographic information systems (GIS) and other specialised software to view and analyse it.

{% assign group = entries | where: "type", "geospatial-and-mapping" | sort_natural: "sort_key" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry show_run_by=false %}
{% endfor %}

## Energy

Generation, demand, pricing and emissions data from Australia's electricity grid.

{% assign group = entries | where: "type", "energy" | sort_natural: "sort_key" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry show_run_by=false %}
{% endfor %}
