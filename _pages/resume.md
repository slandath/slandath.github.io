---
title: "Resume"
layout: single
permalink: /
---

[Download PDF](/Resume.pdf)

## Certifications

{% for certification in site.data.certifications %}
* {{ certification.name }}
{% endfor %}

## Work Experience

{% for job in site.data.jobs %}
### [{{ job.name }}]({{ job.url }}) ({{ job.dates }})

#### {{ job.title }}

{% for bullet in job.bullets %}
* {{ bullet }}
{% endfor %}

{% if job.current_projects %}
#### Current Projects

{% for project in job.current_projects %}
* [{{ project.name }}]({{ project.url }})
{% endfor %}
{% endif %}

{% if job.past_projects %}
#### Past Projects

{% for project in job.past_projects %}
* [{{ project.name }}]({{ project.url }})
{% endfor %}
{% endif %}

{% if job.projects %}
#### Projects

{% for project in job.projects %}
* {{ project }}
{% endfor %}
{% endif %}

{% endfor %}

## Education

### **Michigan State University** (East Lansing, Michigan)

Bachelor of Arts, Philosophy

## Skills

### **Project Management**

Asana, ClickUp, Project Planning, ScrumMaster, Scrum Product Owner, SmartSheets, Waterfall Methodology

### **Software Development**

Agile, GitHub, Jira, Kanban, Trello

### **Web Technologies**

Bash, CSS, Express, Git, Hugo, HTML, JSON, JavaScript, Jekyll, Node.js, Nuxt, REST API, React, SQL, Tailwind CSS, TypeScript, Vue.js, XML
