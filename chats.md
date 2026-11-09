---
layout: category
title: "Community chats"
permalink: /community-chats
last_modified_at: AUTO
data_file: _data/chats.yml
description: .
image: /assets/images/category/chat.png
issue_template: add-entry.yml
---

{% assign entries = site.data["chats"] %}


## Mailing lists

A mailing list sends every message to everyone who subscribed, and you
reply by email. Most keep a public archive you can read first.

{% assign group = entries | where: "type", "mailing-lists" | sort_natural: "name" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}


## Mastodon

Mastodon is a social network made of independent federated servers that talk to each other. If you're interested in the fediverse, there are general-purpose Australian servers like [aus.social](https://aus.social/) and [mastodon.au](https://mastodon.au/).

{% assign group = entries | where: "type", "mastodon" | sort_natural: "name" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}


## Matrix

Matrix is an open standard for chat, so anyone can run a server and any
app can connect to it.

{% assign group = entries | where: "type", "matrix" | sort_natural: "name" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}


## Slack

Slack is a commercial chat tool that some open source projects use for
community conversations.

{% assign group = entries | where: "type", "slack" | sort_natural: "name" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}