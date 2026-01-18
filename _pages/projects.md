---
title: "Projects"
layout: single
permalink: /projects/
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/images/vaporwave-city.jpg
---

## Current

{% for project in site.data.projects %}

### [{{project.name}}]({{project.url}})

{{project.description}}

{% endfor %}

## Past Projects

### [Tazama](https://www.tazama.org/)

A free, open-source software platform dedicated to detecting fraud before it happens.
