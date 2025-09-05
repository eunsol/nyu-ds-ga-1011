---
layout: page
title: Staff
description: A listing of all the course staff members.
---

## Instructor

{% assign instructors = site.staffers | where: 'role', 'Instructor' %}
{% for staffer in instructors %}
{{ staffer }}
{% endfor %}

{% assign teaching_assistants = site.staffers | where: 'role', 'Teaching Assistant' %}
{% assign num_teaching_assistants = teaching_assistants | size %}
{% if num_teaching_assistants != 0 %}
## Teaching Assistants

{% for staffer in teaching_assistants %}
{{ staffer }}
{% endfor %}
{% endif %}


### Please use Discord for most inquiries. If you need to send a private message, please email to fa25-dsga1011-staff@googlegroups.com, which will be read by course instructor and teaching assistants. 
