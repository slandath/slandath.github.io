---
permalink: /projects/
title: "Projects"
---

## Current

{% for project in site.data.projects %}

### [{{project.name}}]({{project.url}})

{{project.description}}

{% endfor %}

## Past Projects

### [Tazama](https://www.tazama.org/)

A free, open-source software platform dedicated to detecting fraud before it happens.
