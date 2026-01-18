---
permalink: /experience/
title: "Experience"
---

## Current

### Program Coordinator at [The Linux Foundation](https://www.linuxfoundation.org/)

A neutral, trusted hub for developers and organizations to code, manage, and scale open technology projects and ecosystems.

## Previous Roles

{% for job in site.data.jobs %}

### {{job.title}} at [{{job.name}}]({{job.url}})

{{job.description}}

{% endfor %}
