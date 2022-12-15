

## Current Schedule

|Day| Time | Location | Type | Distance |
|---|------|----------|------|----------|
{%- for item in site.data.schedule %}
|{{item.day}}|{{item.time}}|[{{item.location}}]({{item.loction_link}})|{{item.type}}|{{item.distance}}|
{%- endfor -%}
