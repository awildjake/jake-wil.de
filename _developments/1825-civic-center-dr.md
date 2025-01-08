---
layout: development_tracking
title: 1825 Civic Center Dr
address: 1825 Civic Center Dr, Santa Clara, CA 95050
developer: Zolman Construction and Development
municipality: Santa Clara
units: 0
phase: Under Review
permits:
    PLN25-00002:
        status: Received
        initial_date: 2025-01-07
        final_date: None
        apn: [22449001]
        address: 1825 Civic Center Dr, Santa Clara, CA 95050
        description: Demolish the existing medical building to create a 8-story multi-family residential building
        names: Zolman Construction and Development;
geometry: ['37.35600299768014', '-121.95693916980261']
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

## In the Meida

- ["Permits Filed For 1825 Civic Center Drive, Santa Clara."](https://sfyimby.com/2025/01/permits-filed-for-1825-civic-center-drive-santa-clara.html) SF YIMBY, January 7, 2025.
