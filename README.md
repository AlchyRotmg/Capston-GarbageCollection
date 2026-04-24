# Corner Brook Garbage Collection Dashboard

A lightweight geospatial decision-support tool for turning a Corner Brook civic address into a clear collection-zone result, an upcoming pickup date, and a readable service view.

This project frames municipal waste collection as a spatial data problem. It links address search, geographic zone boundaries, and calendar rules into one interface so residents can move from location input to service insight in a few seconds.

## Project Snapshot

| Input | Transformation | Output |
| --- | --- | --- |
| Civic address | Geocoding + point-in-polygon zone matching | Collection zone |
| Zone assignment | Schedule lookup | Next pickup date |
| Schedule data | Map and calendar rendering | Resident-facing decision support |

## Analytical Workflow

From a data science perspective, the application behaves like a compact spatial analytics pipeline:
1. Search for a Corner Brook address.
2. Convert the search result into coordinates.
3. Match those coordinates against local collection-zone polygons.
4. Retrieve the correct collection schedule for the resolved zone.
5. Present the outcome through synchronized map and calendar views.

## Core Features

- Address lookup with Corner Brook-focused search behavior
- Geographic zone classification using local boundary data
- Interactive Leaflet map for visual validation of service areas
- Calendar-based pickup schedule display with recycling context
- Local browser persistence for selected address and zone

## Tech Stack

React and Vite power the interface, Leaflet handles spatial visualization, and local zone and schedule datasets provide the service logic behind the dashboard.

## Run Locally

```bash
npm install
npm run dev
```
