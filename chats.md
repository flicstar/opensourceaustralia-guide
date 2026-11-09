---
layout: category
category: community-chats
title: "Community chats"
permalink: /community-chats
data_file: _data/chats.yml
description: "Where the Australian open source community talks: mailing lists, Mastodon servers, Matrix rooms and Slack groups you can join."
image: /assets/images/category/chat.png
issue_template: add-entry.yml
---

{% assign entries = site.data["chats"] %}

Places to talk with other people working on open things in Australia. Plenty of user groups run their own specific chats, for example,
[Flounder](/organisations#flounder) has Matrix rooms, and
[Homelab Brisbane](/organisations#homelab-brisbane) runs a Discourse forum.
Have a look at the organisations and groups you're intested in for more.

## Mailing lists

Email, but to a group. Every message goes to everyone who subscribed, and
you reply by email too. Most lists keep a public archive you can read first.

{% assign group = entries | where: "type", "mailing-lists" | sort_natural: "name" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}


## Mastodon

Mastodon is a social network made of independent, federated servers that talk to each other. You post short messages and follow a feed of other
people's. If you're interested in joining the fediverse, there are general-purpose Australian servers like [aus.social](https://aus.social/) and [mastodon.au](https://mastodon.au/).

{% assign group = entries | where: "type", "mastodon" | sort_natural: "name" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}


## Matrix

Matrix is an open standard for chat, so anyone can run a server and you use an app like [Element](https://element.io/) to connect to it. Conversation happens in rooms you join by topic.

{% assign group = entries | where: "type", "matrix" | sort_natural: "name" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}


## Slack

Slack is a commercial chat tool that some open source projects use for
community conversations. Channels divide things up by topic, and you can reply in a thread, so several conversations can run in one channel at once.

{% assign group = entries | where: "type", "slack" | sort_natural: "name" %}
{% for entry in group %}
  {% include directory-entry.html entry=entry %}
{% endfor %}