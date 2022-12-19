---
layout: page
title: Events
permalink: /events/
---

# Planned Events

{% for event in site.data.events.planned %}

## {{event.name}}

_{{event.date}}_

{{event.description}}
<hr>
{% endfor %}

# Past Events

{% for event in site.data.events.past %}
## {{event.name}}

_{{event.date}}_

{{event.description}}
<hr>
{% endfor %}
