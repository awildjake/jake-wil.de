---
layout: development_tracking
title: 1530 West San Carlos Street
address: 1530 W San Carlos St, San Jose, CA 95126
developer: Urban Villas LLC
municipality: San Jose
units: 237
phase: Approved
permits:
    H22-033:
        status: Approved
        initial_date: 2022-07-22
        final_date: 2023-06-28
        apn: [27718019]
        address: 1530 W San Carlos St, San Jose, CA 95126
        description: Site Development Permit to allow the demolition of three existing commercial buildings, eight unoccupied residential buildings, and associated service structures totaling approximately 14,131 square feet, the removal of 14 trees (11 ordinance-size, three non-ordinance-size) for the construction of an eight-story mixed use building consisting of 237 multifamily residential units and approximately 16,962 square feet of commercial space with an approximately 48% parking reduction on an approximately 1.34 gross acre site.
geometry: ['37.32265813483875', '-121.91826189458949']
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
- [City Website](https://www.sanjoseca.gov/your-government/departments-offices/planning-building-code-enforcement/planning-division/environmental-planning/environmental-review/active-eirs/west-san-carlos-street-project)