---
type: schema
table: episodes
primary_key: path

frontmatter:
  title:
    type: string
    required: true
  date:
    type: date
    required: true
  description:
    type: string
    required: true
  tags:
    type: string[]
    required: true
  extra:
    type: dict
    required: true

h1:
  required: false

sections: {}

rules:
  reject_unknown_frontmatter: false
  reject_unknown_sections: false
  reject_duplicate_sections: false
---

Example

```md
title: Ergonomic updates, digital garden beginnings, and the limits of LLMs
date: 2026-01-09
description: Robin takes us on a tour through his new physical workspace, as well as his digital garden vitual workspace. We both talk about the podcast's schedule, and end on an exploration of what the philosophy of mind can tell us about the limits of LLM reasoning.
tags:
  - ergonomics
  - digital-garden
  - podcasting
  - ai
extra:
  duration: 2565
```
