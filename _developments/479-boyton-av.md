---
layout: development_tracking
title: 479 Boyton Av
address: 479 Boynton Ave, San Jose, CA 95117
developer: Dreamhouse5 Investment LLC
municipality: San Jose
units: 8
phase: Under Review
permits:
    PRE25-007:
        status: Under Review
        initial_date: 2025-01-09
        final_date: None
        apn: [30348020]
        address: 479 Boynton Ave, San Jose, CA 95117
        description: Request preliminary feedback for 8 new three story townhomes.
        names: Ronald Jones w/ Hunt Hale Jones Architects and Dreamhouse5 Investment LLC;
geometry: ['37.31884122484811', '-121.96654969982285']
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
