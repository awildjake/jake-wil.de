---
layout: development_tracking
title: 1050 Saint Elizabeth Street
address: 1050 St Elizabeth Dr, San Jose, CA 95126
developer: Evershine XVII LP
municipality: San Jose
units: 206
phase: Approved
permits:
    H20-049:
        status: Approved
        initial_date: 2021-01-05
        final_date: 2023-04-19
        apn: [28407018]
        address: 1050 St Elizabeth Dr, San Jose, CA 95126
        description: Site Development Permit to allow the demolition of a 28,223 sf two-story commercial building and the construction of a 206-unit 7-story apartment building, with five-stories of residential over two-levels of at grade and partial basement parking, with removal of eight ordinance-size trees and four non-ordinance size trees, on an approximately 2.22-gross acre site in the R-M Multiple Residence Zoning District.
        names: Rocky Shen w/ DNA Design and Architecture; ERIK SCHOENNAUER;
geometry: ['37.30529542068', '-121.91585343694813']
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
- [City Website](https://www.sanjoseca.gov/your-government/departments-offices/planning-building-code-enforcement/planning-division/environmental-review/environmental-review-documents/1050-st-elizabeth-drive-h20-049-er20-270)