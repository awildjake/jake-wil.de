---
layout: development_tracking
title: 849 W San Carlos St
address: 849 W San Carlos St, San Jose, CA 95126
developer: Swenson
municipality: San Jose
units: 64
phase: Under Review
permits:
    PRE24-393:
        status: Under Review
        initial_date: 2024-12-23
        final_date: None
        apn: [26139029]
        address: 849 W San Carlos St, San Jose, CA 95126
        description: To request preliminary feedback for a 64-unit townhome product (assuming no Density Bonus Law) and discuss zoning conformance
        names: Mark Pilarczyk w/ Swenson;
geometry: ['37.32393929654639', '-121.90591281167434']
---

## {{ page.title }}

- Status: {{ page.phase }}
- Units: {{ page.units }}
- Address: {{ page.address }}

## Permits

{% for permit in page.permits %}
  **{{ permit[0] }}** <span class="tag">{{ permit[1].status }}</span>
  >{{ permit[1].description }}
{% endfor %}
