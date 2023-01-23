---
layout: page
title: Routes
permalink: /routes/
---

{% assign routes = site.data.workouts.routes | sort: "distance" %}


<div>
    <table>
        <thead>
            <th>Day</th>
            <th>Time</th>
            <th>Location</th>
            <th>Type</th>
            <th>Distance</th>
        </thead>
        <tbody>
            {%- for route in routes %}
            <tr>
                <td>{{forloop.index}}</td>
                <td><a href="{{route.link}}" target="_blank">Route</a></td>
                <td>{{route.distance}}</td>
                <td>{{route.elevation}}</td>
                <td>{{route.start_point}}</td>
                <td>{{route.tags | join: ", "}}</td>
            </tr>
            {% endfor %}
        </tbody>
    </table>
</div>

## Speedwork

{% for wkt in site.data.workouts.speedwork %}

```
{{wkt.workout}}
```

{% endfor %}

