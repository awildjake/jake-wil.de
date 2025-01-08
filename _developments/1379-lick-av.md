---
layout: development_tracking
title: 1379 Lick Ave
address: 1379 Lick Ave, San Jose, CA 95110
developer: Swenson
municipality: San Jose
units: 74
phase: Under Review
permits:
    PRE24-391:
        status: Under Review
        initial_date: 2024-12-23
        final_date: None
        apn: [43446116]
        address: 1379 Lick Ave, San Jose, CA 95110
        description: To request preliminary feedback on a 74-unit townhome and discuss zoning conformance
        names: Mark Pilarczyk w/ Swenson;
geometry: ['37.31138191797715', '-121.88221240571686']
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
