---
layout: development_tracking
title: West San Carlos Chick-fil-A
address: 1301 W San Carlos St, San Jose, CA 95126
developer: 4G Development & Consulting
municipality: San Jose
units: 0
phase: Under Review
permits:
    H24-046:
        status: Under Review
        initial_date: 2024-08-09
        final_date: None
        apn: [26142059]
        address: 1301 W San Carlos St, San Jose, CA 95126
        description: Site Development permit to allow demolition of existing building and construction of new Chick-fil-a on an approximately 1.09-gross acre site
        names: Hudson Brooks w/ 4G Development & Consulting;
    PRE24-019:
        status: Complete
        initial_date: 2024-01-22
        final_date: 2024-03-01
        apn: [26142059]
        address: 1301 W San Carlos St, San Jose, CA 95126
        description: nhanced Preliminary Review for the demolition of an existing commercial building and the removal of trees for the construction of an approximately 6,005-square-foot quick-serve restaurant (Chik-fil-A) with an outdoor dining patio and 24-hour use (between midnight and 6 a.m.) on an approximately 0.79-gross-acre site.
        names: Hudson Brooks w/ 4G Development & Consulting;
geometry: ['37.32390136676307', '-121.91188690000001']
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
