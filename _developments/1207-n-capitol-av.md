---
layout: development_tracking
title: 1207 N Capitol Avenue
address: 1207 N Capitol Ave, San Jose, CA 95132
developer: DANCO
municipality: San Jose
units: 128
phase: Under Review
permits:
    H24-035:
        status: Under Review
        initial_date: 2024-08-14
        final_date: None
        description: Site development permit to allow the demolition of an existing approximately 5,627-square-foot, single-family house and the removal of14 trees, including four ordinance-size trees, for the construction of a five-story multifamily housing project with 128 affordable housing units, subject to the state Density Bonus law, on an approximately 1.5-gross acre site.
    PRE24-138:
        status: Under Review
        initial_date: 2024-06-04
        final_date: None
        description: SB330 preliminary application to construct 5-story multi-family apartment with 128 affordable units.
geometry: ['37.38805279789893', '-121.86284676747681']
---
# {{ page.title }}
- Status: {{ page.phase }}
- Units: {{ page.units }}
- Address: {{ page.address }}

## Description
DANCO is proposing a 100% affordable, five-story multifamily housing project with 128 affordable housing units on a 1.5-gross acre site in San José's Berryessa District. The project will provide affordable units for households and individuals earning between 30 and 70% of the Area Median Income. Residents will have access to 55 parking spaces in an at-grade parking lot as well as 55 long-term bicycle storage spaces and scattered short-term bicycle parking. Additional proposed amenities include a community kitchen, fitness room, yoga studio, and cafe space.

## Permits

{% for permit in page.permits %}
  **{{ permit[0] }}** ({{ permit[1].status }})
  >{{ permit[1].description }}
{% endfor %}

