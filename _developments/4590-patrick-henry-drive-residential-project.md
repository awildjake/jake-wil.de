---
layout: development_tracking
title: 4590 Patrick Henry Drive Residential Project
address: 4590 Patrick Henry Dr, Santa Clara, CA 95054
developer: KASA Partners
municipality: Santa Clara
units: 284
phase: Under Review
permits:
    PRE23-00139:
        status: Approved
        initial_date: 2023-06-06
        final_date: 2024-11-19
        apn: [10404123]
        address: 4590 Patrick Henry Dr, Santa Clara, CA 95054
        description: Tentative Parcel Map to subdivide the existing parcel into two parcels. Parcel 2 will be dedicated to the City. Development proposal for 2.79 acre parcel at 4590 Patrick Henry Drive to entitle 284 multifamily units, including 15% affordable, and dedicate 0.55 acre park
        names: James Suh
geometry: ['37.396914991265746', '-121.98564348650464']
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
