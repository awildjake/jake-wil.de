---
layout: development_tracking
title: 546 Bird Ave
address: 546 Bird Ave., San Jose, CA 95125
developer: Ver Consultants
municipality: San Jose
units: 16
phase: Under Review
permits:
    PRE24-384:
        status: Under Review
        initial_date: 2024-12-18
        final_date: None
        apn: [26418052]
        address: 546 Bird Ave., San Jose, CA 95125
        description: Enhanced Preliminary Review to construct a 16-unit multifamily residential development.
        names: Vince Rivero w/ VER CONSULTANTS;
geometry: ['37.32090542906241', '-121.89802120688186']
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