---
layout: development_tracking
title: 4220 Network Circle
address: 4220 Network Cir, Santa Clara, CA 95054
developer: Valley Oak Partners
municipality: Santa Clara
units: 584
phase: Under Review
permits:
    PLN24-00136:
        status: In Review
        initial_date: 2024-03-15
        final_date: None
        apn: [09708058]
        address: 4220 Network Cir, Santa Clara, CA 95054
        description: Builder’s Remedy Application to develop the 38-acre site with a total of 584 units - 120 affordable apartments, 416 townhomes in three distinct neighborhoods in combination of 48 single-family dwellings with open space and parking spaces. “NETWORK CIRCLE” PROJECT DESCRIPTION - OVERALL Valley Oak Partners is excited to present this 38-acre residential development encompassing a diverse array of housing types connected by a sophisticated network of open spaces. The plan includes 120 affordable apartments, 416 townhomes in 3 distinct neighborhoods, and 48 single family homes. The design concept for the project is focused on open space. A unique aspect of this plan is the generous amount of open space – a 2.6 acre active park on the western edge of the site, a 2.3 acre park at the heart of the site adjacent to the historic Clock Tower. In addition, the project features a 1.3 acre green belt/linear park (running on the southern property line from west to east) and a 0.5 acre green belt/linear park (running north to south) that links together the parks and neighborhoods. Additionally, the project’s open space connects to the 14.9 acre Agnews Historic Park creating an extensive open space network. The project’s open space was also strategically sited to preserve a large amount of the property’s existing trees. Multiple large open spaces provide for both active and passive uses. Active uses include a soccer field, a basketball court, play structures for kids, and multiple dog parks. The Clock Tower park programming skews a little more passive to complement and be sympathetic to the existing historical uses. Open spaces will be planted with a range of native and drought tolerant species. The wide range of housing types is matched by a diversity of architectural styles. The affordable apartments and 3 story townhomes embrace a warm and modern aesthetic that gives a distinct character to the heart of the site, while the 2 story townhomes and single-family homes take on a more traditional look appropriate to the more intimate scale of the western portion of the site.
geometry: ['37.39183503151553', '-121.95318954233022']
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
