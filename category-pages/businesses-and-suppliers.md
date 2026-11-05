---
layout: category
category: businesses-and-suppliers
title: "Businesses and suppliers"
permalink: /businesses-and-suppliers
description: Australian businesses offering development, hosting, support, training and hardware for open source software, data and research.
image: /assets/images/category/handshake.png
issue_template: add-business.yml
issue_link_label: "Add your business"
---

{% assign entries = site.data.category_data["businesses-and-suppliers"] %}

Using open source is generally free. Getting help with it is not, and paying someone to help you is normal. A service provider can migrate your systems, host them, fix them, build something new, or train your team. Others sell you the gear: computers with Linux already installed, or open hardware to build with.

A listing on this page is not an endorsement. You still need to ask your own questions before you engage anyone.

If you run a business that belongs here, it’s free to add your listing. You must have an Australian presence, and you'll need to include what open source projects or tools you use, the services you provide, and what sector you usually work with (for example, small business, government, schools, not for profits).

## Infrastructure and cloud

{% assign group = entries | where: "type", "infrastructure-and-cloud" | sort_natural: "slug" %}
{% for entry in group %}
  {% include businesses-and-suppliers-entry.html entry=entry %}
{% endfor %}

## Learning and collection systems

{% assign group = entries | where: "type", "learning-and-collection-systems" | sort_natural: "slug" %}
{% for entry in group %}
  {% include businesses-and-suppliers-entry.html entry=entry %}
{% endfor %}

## Open hardware suppliers

{% assign group = entries | where: "type", "open-hardware-suppliers" | sort_natural: "slug" %}
{% for entry in group %}
  {% include businesses-and-suppliers-entry.html entry=entry %}
{% endfor %}


## Web and content management

Plenty of web agencies in Australia work with open source CMSs. You can find Drupal agencies based in, or serving, Australia on their [Organizations page](https://new.drupal.org/organizations?title=&loc_served%5B%5D=27573){:target="_blank"}.

{% assign group = entries | where: "type", "web-and-content-management" | sort_natural: "slug" %}
{% for entry in group %}
  {% include businesses-and-suppliers-entry.html entry=entry %}
{% endfor %}