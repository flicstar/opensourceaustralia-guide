---
layout: category
category: open-data
title: "Open Data"
permalink: /open-data
description: "Australian open data: government portals, civic tech, GLAM collections, research and spatial data."
---

{% assign entries = site.data.category_data["open-data"] %}

Open data is information that anyone can access, use and share, released under a
licence that says so.
 
A dataset can be openly licensed without any software attached to it, and often is: a spreadsheet of census figures, a map
layer of soil types, a list of every planning application lodged in your council
area.
 
You might be surprised by how much is already freely available to you. Some of
it downloads as a file. Some of it comes through an API, which is a way for one
program to ask another program for data, so a developer can build something that
stays up to date without anyone re-downloading anything.
 
Australia has a government open data policy, and CC BY is the default licence
for Australian Government data. Read the
[Australian Government Public Data Policy Statement](https://www.pmc.gov.au/resources/public-data-policy-statement).
 
There's no single place all of it lives. Publishing is split across federal
agencies, state and territory governments, universities and research bodies, and
volunteer-run community projects. 

## Government portals

Every level of government publishes data, and each runs its own catalogue. The
federal catalogue aggregates some state and local material, but not all of it, so
it's worth checking your state portal directly.

{% assign group = entries | where: "type", "government-portals" | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}

## Civic tech

Civic tech projects take government information that that anyone can see but few can use, and republish it in a form people can actually work with. Australia's
civic tech sector is small. Much of it runs on volunteer time and donations.

{% assign group = entries | where: "type", "civic-tech" | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}

## GLAM

GLAM stands for Galleries, Libraries, Archives and Museums. Open GLAM is a
movement for free and open access to digital cultural heritage: the collections,
catalogues and digitised material that these institutions hold.

{% assign group = entries | where: "type", "glam" | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}

## Transport
 
Timetables, stop locations, real-time vehicle positions and road network data.
Most Australian transport agencies publish in GTFS, an open standard for
transit data.

{% assign group = entries | where: "type", "transport" | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}

## Sciences and geospatial
 
Spatial data is any information with a location attached to it, describing where
something is and what shape and size it takes. You use geographic information
systems (GIS) and other specialised software to view and analyse it. Australia's
science agencies and research infrastructure programs publish theirs openly, along
with biodiversity, marine, soil and elevation data.

{% assign group = entries | where: "type", "sciences-geospatial" | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}

## Research data and open access
 
Open access means published research that anyone can read without paying for it.
Open research data is the material behind those publications. Australian
universities each run their own repository, and national infrastructure connects
them. For the history of how open access developed here, see
[Open access in Australia](https://en.wikipedia.org/wiki/Open_access_in_Australia)
on Wikipedia.

{% assign group = entries | where: "type", "research-dat" | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}

## Events

{% assign tagged = site.data.events | where_exp: "e", "e.tags contains 'open-data'" | sort_natural: "slug" %}
{% for entry in tagged %}
  {% include directory-entry.html entry=entry %}
{% endfor %}