---
layout: development_tracking
title: Santa Clara Park
address: 2518 Mission College Blvd, Santa Clara, CA 95054
developer: Irvine Company
municipality: Santa Clara
units: 1792
phase: Under Review
permits:
    PLN24-00160:
        status: In Review
        initial_date:
        final_date:
        apn: []
        address:
        description: General Plan Amendment, Rezoning and Architectural Review to construct 1,792 apartment units with approximately 1,747,900 square feet of residential buildings and 1,087,930 square feet of garage and 3,500 SF of retail space on a 25.74-acre parcel in Freedom Circle Focus Area.
        names:
geometry: ['37.38857043777823', '-121.97050610000002']
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
