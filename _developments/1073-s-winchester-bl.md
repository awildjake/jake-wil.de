---
layout: development_tracking
title: 1073 South Winchester Boulevard
address: 1073 S Winchester Blvd, San Jose, CA 95128
developer: A&Z Development
municipality: San Jose
units: 61
phase: Approved
permits:
    SP20-002:
        status: Approved
        initial_date: 2024-08-14
        final_date: 2021-08-25
        description: Special Use Permit to allow demolition of two buildings totaling 9,762 square feet and allow the construction of a 6-story mixed-use building consisting of 61 residential condo units and approximately 17,970 square feet of commercial space, and allow the removal of 9 ordinance size trees and 7 non-ordinance size trees on a 0.82-gross acre site, in the Winchester Boulevard Urban Village.
geometry: ['37.30717545930334', '-121.95037008578649']
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

## Links
- [City Website](https://www.sanjoseca.gov/your-government/departments-offices/planning-building-code-enforcement/planning-division/major-development-projects/1073-s-winchester-boulevard)