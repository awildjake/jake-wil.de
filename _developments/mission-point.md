---
layout: development_tracking
title: Mission Point
address: 3005 Democracy Way, Santa Clara, CA 95054
developer: Kylli
municipality: Santa Clara
units: 2800
phase: Approved
permits:
    PLN2017-12924:
        status: Approved
        initial_date:
        final_date:
        apn: []
        address:
        description: General Plan Amendment from the High-Intensity Office/Research and Development (R&D) to a new designation allowing high-intensity mixed use development, including residential and office
        names:
geometry: ['37.40270785432979', '-121.98195799999998']
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
