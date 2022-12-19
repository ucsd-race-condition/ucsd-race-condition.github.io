---
layout: page
title: Routes
---

{% assign routes = site.data.workouts.routes | sort: "distance" %}

|#|Map|Distance|Elevation|
|----|--------|---------|
{%- for route in routes %}
|{{forloop.index}}|[Route]({{route.link}}){:target="_blank"}|  {{route.distance}} | {{route.elevation}} |
{%- endfor %}



## Speedwork

{% for wkt in site.data.workouts.speedwork %}

```
{{wkt.workout}}
```

{% endfor %}

