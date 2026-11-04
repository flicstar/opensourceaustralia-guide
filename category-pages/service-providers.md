---
layout: category
category: service-providers
title: "Service providers"
permalink: /service-providers
description: Australian businesses offering migration, hosting, support, development and training for open source software, hardware and data
image: /assets/images/category/handshake.png
---

{% assign entries = site.data.category_data["service-providers"] %}

Using open source is generally free. Getting help with it is not, and paying someone to help you is normal. A service provider can migrate your systems, host them, fix them, build something new, or train your team. Some work with software, others work with hardware, data, or open standards.

A listing on this page is a record, not an endorsement. You still need to ask your own questions before you engage anyone.

If you run a business that belongs here, it’s free to add your listing. You must have an Australian presence, and you'll need to include what open source projects or tools you use, the services you provide, and what sector you usually work with (for example, small business, government, schools, not for profits).

[**Add your business**](https://github.com/flicstar/opensourceaustralia-guide/issues/new?template=add-business.yml)

## Infrastructure and cloud

{% assign group = entries | where: "type", "infrastructure-and-cloud" | sort_natural: "slug" %}
{% for entry in group %}
  {% include service-provider-entry.html entry=entry %}
{% endfor %}

## Learning and collection systems

{% assign group = entries | where: "type", "learning-and-collection-systems" | sort_natural: "slug" %}
{% for entry in group %}
  {% include service-provider-entry.html entry=entry %}
{% endfor %}

## Web and content management

{% assign group = entries | where: "type", "web-and-content-management" | sort_natural: "slug" %}
{% for entry in group %}
  {% include service-provider-entry.html entry=entry %}
{% endfor %}