---
layout: development_tracking
title: 19601 McKean Road
address: 19601 McKean Rd, San Jose, CA 95120
developer: The Landmark Developers
municipality: Santa Clara County
units: 99
phase: Under Review
permits:
    PLN24-249-PRE:
        status: In review
        initial_date: 2024-12-11
        final_date: None
        apn: [70136040]
        address: "This is the Preliminary Application Pursuant to SB 330 for 99 residential units with a total residential development square footage of 257,540 Sq Ft. Three housing types are being proposed: Townhouses (33), Duplexes (16 units), and Single Family Homes (50) of varying sizes. The proposed development contains 20% Affordable Housing at the Low Income Level, which will be 20 townhouses. All residential units will be entitled to a front yard, a rear yard, and a parking space. All residences will also have additional parking as the streets are designed to accommodate on-street parking. There will be a total of approximately 469 total parking spots [148 Garage Spots, 181 Driveway Spots, and approximately 140 street parking spots]."
        names: Owners are Rakesh & Paulomi Patel;
geometry: ['37.197398327288944', '-121.80421075767205']
---

## {{ page.title }}

- Status: {{ page.phase }}
- Units: {{ page.units }}
- Address: {{ page.address }}

## Details

This most recent permit for this project was submitted with Santa Clara County.

## Permits

{% for permit in page.permits %}
  **{{ permit[0] }}** <span class="tag">{{ permit[1].status }}</span>
  >{{ permit[1].description }}
{% endfor %}

## In the Community

This project was covered by [SF YIMBY](https://sfyimby.com/2024/12/sb-330-filed-for-housing-at-19601-mckean-road-san-jose.html) on January 6, 2025.
