---
layout: development_tracking
title: 2610 El Camino Real
address: 2610 E El Camino Real, Santa Clara, CA 95051
developer: Toll Brothers
municipality: Santa Clara
units: 601
phase: Under Review
permits:
    PLN24-00504:
        status: In Review
        initial_date: 2024-10-01
        final_date: None
        apn: [29006020]
        address: 2610 EL CAMINO REAL, SANTA CLARA CA 95051
        description: This project on the existing Moonlite Center site at 2640 El Camino Real consists of the re-development of an approximately 14.34 acre existing retail commercial site. The current strip mall development will be transformed into a vibrant housing complex with 601 dwelling units, and over 60,000 SF of open space. The following submittal drawings are the basis for the City of Santa Clara SB-330 formal Application. The site incorporates a multimodal transportation network consistent with the City’s vision focusing on complete streets, allowing for safe and convenient transportation suitable for all modes of travel. The new development locates the larger and taller buildings along the frontage of El Camino Real along a large plaza. As the site transitions into the adjacent residential neighborhoods to the South, the scale of the building steps down to Townhomes three stories tall, similar in scale to the recent adjacent development. Three 6-7 story buildings are sited along El Camino Real – two condominium buildings with 140 and 136 units each and one below market rate rental apartment building with 166 units. Parking is provided internally within these buildings with 2 level garages that are lined with active uses on the ground floors facing the streets. Along the Southern half of the site, the new development includes 159 three story Townhomes similar in scale to the recent development on Keily Blvd. The Townhomes include private entrances at the ground floor as well as two car private garages. The new development is anchored around a central plaza which links El Camino Real with the core of the development. The central open space transitions from more urban uses fronting along El Camino to a more neighborhood residential park as it moves into the center of the development. The development includes a mix of dwelling types including Townhomes, Condominiums as well as below market rate rental apartments. Approximately 27% below market rate rental apartments are included in the overall development. There is also a mix of unit sizes with 1, 2 and 3 bedroom units in both the condo buildings and the affordable rental apartment building. The Townhomes will include flexibility in the floor plans with a mix of 2+ and 3 bedroom units. This development will bring an infusion of activity to the area. The mix of residential and related amenity/support uses together with the pedestrian orientation of the design and open spaces will be an asset to the neighborhood and to the City of Santa Clara. At the time of construction, Toll Brothers anticipates site activity to take place during the hours of 7:00 AM to 5:00 PM and expects a range of 50 to 250 employees onsite in full production, contingent on the development activity taking place.
        names: Toll Brothers
geometry: [37.351907460603606, -121.9737361994423]
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