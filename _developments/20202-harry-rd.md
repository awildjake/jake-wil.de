---
layout: development_tracking
title: 20202 Harry Rd
address: 20202 Harry Rd, San Jose, CA 95120
developer: GAVELLO GAIL A TRUSTEE & ET AL, In Care Of JOHN J. DITO & SON
municipality: Santa Clara County
units: 177
phase: Under Review
permits:
    PLN24-119-PRE:
        status: Complete
        initial_date:
        final_date:
        apn: []
        address:
        description: SB330 Pre-Application for a 177-lot subdivision to include single family detached homes and duet residential units, reservation of various non-buildable parcels for open space and utilities. Total residential area totals 533,176 sq.ft. (living - 435,172 + garage - 98,004).
        names:
geometry: ['37.203428000036176', '-121.82526945766976']
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
