---
layout: development_tracking
title: 3521 Homestead Road
address: 3521 Homestead Rd, Santa Clara, CA 95051
developer: Waymark
municipality: Santa Clara
units: 153
phase: Under Review
permits:
    PLN24-00633:
        status: Received
        initial_date: 2024-12-02
        final_date: None
        apn: [29023049, 29023053]
        address: 3521 Homestead Rd, Santa Clara, CA 95051
        description: The applicant is seeking planning review of the proposed redevelopment of a 2-parcel assemblage comprised of an approximate 5.55-acre retail strip center located at the intersection of Homestead Road and Lawrence Expressway in Santa Clara. The property, consisting of two parcels at 3521 and 3591 Homestead Road (APN’s 290-23-049 and 290-23-053), is currently designated Neighborhood Mixed Use (NMU) in the City’s General Plan. This designation allows for 20 dwellings per acre minimum to 36 dwelling units per acre maximum with 0.10 FAR of commercial, and zoned Community Commercial (CC). The applicant is proposing a 153-unit residential project, aligning with the General Plan’s residential density range of 20-36 dwellings per acre, specifically proposing 27.5 dwellings per acre. This project includes (90) 4-story stacked townhomes and (63) 3-story townhomes.
        names: Waymark;
geometry: ['37.339153480676366', '-121.9943127601609']
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
