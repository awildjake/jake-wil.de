---
layout: development_tracking
title:
address:
developer:
municipality:
units:
phase:
permits:
    PRE23-00139:
        status:
        initial_date:
        final_date:
        apn: []
        address:
        description:
        names:
geometry: []
---
# {{ page.title }}
- Status: {{ page.phase }}
- Units: {{ page.units }}
- Address: {{ page.address }}

## Permits
{% for permit in page.permits %}
  **{{ permit[0] }}** ({{ permit[1].status }})
  >{{ permit[1].description }}
{% endfor %}