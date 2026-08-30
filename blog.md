---
layout: page
title: "Blog"
permalink: /blog
description: "Writing about open source in Australia."
---

This page will hold writing about open source in Australia: what is happening here, what other countries are doing, and what that suggests for us.

<span>{% include icons/construction.svg %}</span> Checkout my [Research backlog](https://github.com/flicstar/opensourceaustralia-guide/blob/main/RESEARCH-BACKLOG.md#blog-posts){:target="_blank"} file to see what blog posts I'm planning, and let me know your ideas. {% include icons/construction.svg %}


{% for post in site.posts %}
  <article class="post-item">
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <p class="post-date">{{ post.date | date: "%-d %B %Y" }}</p>
  </article>
{% endfor %}