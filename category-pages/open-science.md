---
layout: category
category: open-science
title: "Open science"
permalink: /open-science
---

{% assign entries = site.data.category_data["open-science"] %}

Open science means research that anyone can read, check and build on. That covers the publications, the data behind them, and the methods used to get there.

This page covers all disciplines, not just the natural sciences. You might see the term "open scholarship" used when people want to be explicit about including humanities.

## Research data collections

Collections that hold research data you can use.

{% assign group = entries | where: "type", "research-data-collection" | sort_natural: "sort_key" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry show_run_by=false %}
{% endfor %}

## Catalogues and search

These catalogues index data that's held elsewhere, so you can search across many institutions at once.

{% assign group = entries | where: "type", "catalogue-search" | sort_natural: "sort_key" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry show_run_by=false %}
{% endfor %}

## Open access publishing

Open access means published research that anyone can read without paying for it. Jack McKenna gives a summary of [Open Access in Australia](https://blog.mdpi.com/2024/11/26/open-access-in-australia/){:target="_blank"} on the MDPI blog, and you can read the [history of how open access developed here](https://en.wikipedia.org/wiki/Open_access_in_Australia){:target="_blank"} on Wikipedia.

{% assign group = entries | where: "type", "open-access" | sort_natural: "sort_key" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry show_run_by=false %}
{% endfor %}

## Open methods

Open methods means sharing how the research was done, not just what it found. That covers the step-by-step protocols, the analysis code, and the software the work depends on.

{% assign group = entries | where: "type", "open-methods" | sort_natural: "sort_key" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry show_run_by=false %}
{% endfor %}
