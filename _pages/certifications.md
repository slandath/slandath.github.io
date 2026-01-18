---
title: "Certifications"
layout: single
permalink: /certifications/

header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/images/vaporwave-city.jpg
---

{% include feature_row %}

{% for certification in site.data.certifications %}

### [{{certification.name}}]({{certification.url}})

{{certification.description}}

{% endfor %}
