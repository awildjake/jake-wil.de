---
layout: development_tracking
title: 255 W Julian St
address: 255 W Julian St, San Jose, CA 95110
developer: Westbank
municipality: San Jose
units: 0
phase: Under Review
permits:
    H24-049:
        status: Under Review
        initial_date: 2024-08-27
        final_date: None
        apn: [25931071]
        address: 255 W Julian St, San Jose, CA 95110
        description: "Site Development Permit to allow either Option A, which consists of the construction of a 14-story office building with ground-floor retail space and four underground parking levels and modification of an existing six-story office building to change the ground-floor use to retail and make changes to the facade, as approved under SP21-037, or Option B, which consists of the construction of an 18-story residential tower with four levels of underground parking and approximately 13,100 square feet of ground-floor retail space, on an approximately 1.8-gross-acre site."
        names: Project West Julian LLC; Westbank
geometry: ['37.33775966978271', '-121.89671618895639']
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
