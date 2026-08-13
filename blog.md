---
layout: page
title: "Blog"
permalink: /blog
description: "Writing about open source in Australia."
---

This page will hold writing about open source in Australia: what is happening here, what other countries are doing, and what that suggests for us. 

{% for post in site.posts %}
  <article class="post-item">
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <p class="post-date">{{ post.date | date: "%-d %B %Y" }}</p>
  </article>
{% endfor %}