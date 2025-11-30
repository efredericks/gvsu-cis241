---
layout: page
title: Instructor
description: A listing of all the course staff members.
nav_order: 3
---

## Instructors

{% assign instructors = site.staffers | where: 'role', 'Instructor' %}
{% for staffer in instructors %}
{{ staffer }}
{% endfor %}

