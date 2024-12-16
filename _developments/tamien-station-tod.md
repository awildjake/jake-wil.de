---
layout: development_tracking
title: Tamien Station Transit Oriented Development
address: 1197 Lick Ave, San Jose, CA 95110
developer: Republic Urban
municipality: San Jose
units: 434
phase: Approved
permits:
    PD20-003:
        status:
        initial_date:
        final_date:
        apn: []
        address:
        description: Planned Development Permit to allow the demolition of a 11,400 square foot building and construction of a mixed-use development consisting of 569 residential units (Option A) or 555 residential units (Option B) within three buildings, up to 3,000 square feet of child day care or commercial space and the removal of 64 ordinance sized trees and 58 Non-Ordinance sized trees on a 6.96 gross acre site.
        names:
geometry: ['37.31221138453271', '-121.88316703764922']
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
