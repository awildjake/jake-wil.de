---
layout: development_tracking
title: 1520 West San Carlos Street
address: 1520 W San Carlos St, San Jose, CA 95126
developer: Vivji Mani / Urban Villas LLC
municipality: San Jose
units: 256
phase: Approved
permits:
    H23-004:
        status: Approved
        initial_date: 2021-03-19
        final_date: 2023-07-12
        apn: [27718021]
        address: 1520 W SAN CARLOS ST SAN JOSE, CA 95126-3235
        description: Site Development Permit to allow the demolition of two commercial buildings, 11 residential buildings, and two service structures totaling approximately 7,926 square feet and the removal of 29 trees (27 ordinance-size, 2 non-ordinance-size) for the construction of an 8-story mixed use building consisting of 256 multifamily residential units (39 affordable units) and approximately 15,203 square feet of commercial space with an approximately 38% parking reduction on an approximately 1.62-gross acre site.
        names: Viji Mani w/ Urban Villas LLC; 
geometry: ['37.32322919513452', '-121.91787443954438']
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
- [City Website](https://www.sanjoseca.gov/your-government/departments-offices/planning-building-code-enforcement/planning-division/environmental-planning/environmental-review/negative-declaration-initial-studies/1520-west-san-carlos-mixed-use-project)