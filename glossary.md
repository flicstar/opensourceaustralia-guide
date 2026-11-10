---
layout: glossary
title: "Glossary"
permalink: /glossary
data_file: _data/glossary-terms.yml
description: "Plain-language definitions for terms used across this site: licensing, community, open data, hardware, standards, open science, AI and more."
image: /assets/images/category/glossary.png
issue_template: add-entry.yml
---

Here are the terms used across this site defined in plain language. Most of these terms have a Wikipedia article if you want to read further.

<span>{% include icons/construction.svg %}</span> Turns out glossaries are hard! This is going to take me while. 😬  {% include icons/construction.svg %}

## Other glossaries

There are many other specialist glossaries you can refer to that go deeper on particular corners of open source.

* [Open {re}Source glossary](https://openresource.dev/guide/glossary/). Terms used by people contributing to and maintaining projects.
* [Open Data Handbook glossary](https://opendatahandbook.org/glossary/en/). Open data terms.`
* [Open Access Australasia](https://oaaustralasia.org/definitionsrr/). Open access and author rights.

{% assign entries = site.data["glossary-terms"] %}

## Terms

{% assign letters = "A|B|C|D|E|F|G|H|I|J|K|L|M|N|O|P|Q|R|S|T|U|V|W|X|Y|Z" | split: "|" %}
{% assign sorted_entries = entries | sort_natural: "name" %}
{% for letter in letters %}

### {{ letter }}

{% assign letter_lower = letter | downcase %}
{% for entry in sorted_entries %}
  {% assign entry_initial = entry.name | slice: 0 | downcase %}
  {% if entry_initial == letter_lower %}
{% include glossary-entry.html entry=entry %}
  {% endif %}
{% endfor %}
{% endfor %}
