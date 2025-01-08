---
layout: development_tracking
title: 10333 N Wolfe Road
address: 10333 N Wolfe Rd, Cupertino, CA 95014
developer: Eden Housing
municipality: Cupertino
units: 249
phase: Under Review
permits:
    PR-2024-074:
        status: In review
        initial_date: 2024-12-17
        final_date: None
        apn: [31620088]
        address: 10333 N Wolfe Rd, Cupertino, CA 95014
        description: 249 units of rental workforce housing spread across seven buildings on a 5.16-acre parcel. The project will include 219 parking spaces split across surface parking and a concrete parking podium. The project will also contain a variety of outdoor spaces and a portion of the Tamien Innu bicycle-pedestrian trail.
        names: Eden Housing;
geometry: ['37.32976709933505', '-122.01593556244406']
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

## In the Media

- ["Preliminary Permits for Freeway-Adjacent Housing in Cupertino."](https://sfyimby.com/2025/01/preliminary-permits-for-freeway-adjacent-housing-in-cupertino.html) SF YIMBY, January 6, 2025.
