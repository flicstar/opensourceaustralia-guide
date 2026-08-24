---
layout: category
category: open-science
title: Open science
permalink: /open-science
---

{% assign entries = site.data.category_data["open-science"] %}

Open science is a broad term that covers all systematic scholarship including natural sciences as well as history and philosophy. This page covers research across all disciplines. You might see the term "open scholarship" used when people want to be explicit about including humanities.

Checkout my [Research backlog](https://github.com/flicstar/opensourceaustralia-guide/blob/main/RESEARCH-BACKLOG.md){:target="_blank"} file to see what I've captured so far, and let me know what I've missed.

{% comment %}

## Research data collections
 
{% assign group = entries | where: "type", "research-data-collection" | sort_natural: "sort_key" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry show_run_by=false %}
{% endfor %}

## Finding and accessing research

Blurb that mentions open access publishing and open methods. Open access means published research that anyone can read without paying for it.
Open research data is the material behind those publications. Australian
universities each run their own repository, and national infrastructure connects
them. For the history of how open access developed here, see
[Open access in Australia](https://en.wikipedia.org/wiki/Open_access_in_Australia)
on Wikipedia.

{% assign group = entries | where: "type", "finding-research" | sort_natural: "sort_key" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry show_run_by=false %}
{% endfor %}

{% endcomment %}