---
layout: development_tracking
title: 595 Park Ave
address: 595 Park Ave, San Jose, CA 95110
developer: Manu Studios
municipality: San Jose
units: 8
phase: Under Review
permits:
    PRE24-323:
        status: Complete
        initial_date: 2024-11-21
        final_date: 2025-01-08
        apn: [25948057]
        address: 595 Park Ave, San Jose, CA 95110
        description: Focused Preliminary Review to allow the conversion of the existing three-story approximately 13,405-square-foot building into a mixed-use building consisting of ground floor retail space, office space, eight residential units, and amenity space on an approximately 0.56-gross-acre site.
        names: Yining Luo w/ Manu Studios & 595 Park Avenue LLC;
geometry: ['37.32686559707847', '-121.90042201232401']
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
