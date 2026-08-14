---
layout: post
title: "What is open data?"
tags:
  - "open-data"
---

## Hello world

Lorem ipsum

## Heading two

And another pagaraph.

## Syntax test

YAML, the one that matters:

```yaml
# Government portals
- slug: "data-gov-au"
  name: "data.gov.au"
  url: "https://data.gov.au/"
  type: "government-portals"
  sort_key: "010"
  status: "active"
  count: 140000
  verified: true
  description: |
    The central catalogue of Australian open government data.
```

Liquid, to check tags and filters:

```liquid
{% assign portals = entries | where: "type", "government-portals" | sort_natural: "sort_key" %}
{% for entry in portals %}
  {% include directory-entry.html entry=entry %}
{% endfor %}
```

SCSS, to check nesting and properties:

```scss
.entry-name {
  font-family: var(--font-display);
  font-size: 1.125rem;

  a:hover {
    color: var(--link-hover); // should be plum-free
  }
}
```

Shell, since contributing docs always have some:

```bash
bundle exec jekyll serve --livereload
```