---
layout: category
category: open-source-software
title: Open source software
permalink: /open-source-software
---

{% assign entries = site.data.category_data["open-source-software"] %}

Open source software means the source code for the software is available for anyone to read, change, and share. This is in direct contrast to proprietary or closed-source software like Microsoft Word or Spotify.

You might also see the terms *free software*, and *free and open source software (FOSS)*. See [What is Open Source](what-is-open-source.md) for how these terms differ.

Australia has a long history of building and maintaining open source software. Some of it you probably even use today. This page lists software with Australian origins and projects that have been shaped in a serious way by Australians.

<span>{% include icons/construction.svg %}</span> Checkout my [Research backlog](https://github.com/flicstar/opensourceaustralia-guide/blob/main/RESEARCH-BACKLOG.md#open-source-software){:target="_blank"} file to see what I've captured so far, and let me know what I've missed. {% include icons/construction.svg %}

{% comment %}

## Civic and community tools

Software for running elections, scraping public data, and other work in the public interest.

{% assign group = entries | where: "type", "civic-and-community-tools" | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}

## Communications

Phone systems and the codecs that carry voice over a network.

{% assign group = entries | where: "type", "communications" | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}

## Data and monitoring

Tools for collecting data and watching what your systems are doing.

{% assign group = entries | where: "type", "data-and-monitoring" | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}

## Desktops and window managers

The part of an operating system you look at and click on.

{% assign group = entries | where: "type", "desktops-and-window-managers" | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}

## Education

Software for teaching and running courses.

{% assign group = entries | where: "type", "education" | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}

## Networking and file sharing

Moving files between machines and controlling what travels across a network.

{% assign group = entries | where: "type", "networking-and-file-sharing" | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}

## Operating systems and firmware

The software underneath everything else, from full Linux distributions to the code that runs on a single chip.

{% assign group = entries | where: "type", "operating-systems-and-firmware" | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}

## Robotics and autonomous vehicles

Software that makes machines move on their own.

{% assign group = entries | where: "type", "robotics-and-autonomous-vehicles" | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}

## Security

Tools for finding and analysing threats.

{% assign group = entries | where: "type", "security" | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}

## Software development

Tools you use while you are writing code.

{% assign group = entries | where: "type", "software-development" | sort_natural: "slug" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}


{% endcomment %}