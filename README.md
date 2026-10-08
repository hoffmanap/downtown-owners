# Who Owns Downtown El Paso

An interactive parcel-level ownership map of downtown El Paso, in the spirit of a [Knakal map](https://www.bkrea.com/knakal-map-room): every lot drawn to its real footprint, colored by ownership network rather than by individual owner, so scattered LLC/shell-entity holdings read as one connected network instead of requiring manual toggling.

**[View the live map](https://hoffmanap.github.io/downtown-owners/)**

## What it shows

- 1,636 downtown parcels, each drawn to its real lot footprint (pulled from the City of El Paso's parcel GIS) or as a point where no footprint is available
- 87 ownership networks identified by shared mailing address and/or name-matching, with the largest 26 (72% of all clustered value) confirmed where possible via TX Comptroller / SOSDirect / OpenCorporates registered-agent lookups
- Thin threads connecting each network's scattered parcels so the shape of a holding is visible at a glance
- Toggleable layers: aerial imagery, street-name labels, and a georeferenced 1908 Sanborn fire-insurance-map overlay (tiled live from UT Austin's public-domain scans) showing what stood on each lot over a century ago
- An opacity slider for the ownership layer, to see the aerial or historical map underneath

## Data sources

- Parcel ownership, assessed value, and mailing address: Regrid / El Paso Central Appraisal District
- Parcel footprints: [City of El Paso GIS (EPParcels)](https://gis.elpasotexas.gov/arcgis/rest/services/EPParcels/FeatureServer)
- 1908 Sanborn Fire Insurance Maps: [UT Austin Libraries GeoData](https://geodata.lib.utexas.edu/), public domain, tiled via [titiler.xyz](https://titiler.xyz)
- Aerial imagery / street labels: Esri World Imagery and Esri Reference services (free, no key)
- Beneficial-ownership confirmations: manual TX Comptroller Franchise Tax / SOSDirect / OpenCorporates lookups

## Notes

- A cluster means entities share a mailing address and/or have near-identical names in the appraisal record — not confirmed common beneficial ownership in every case. Badges on the map distinguish "CONFIRMED" (a human matched an officer/registered-agent record) from "INFERRED" (address/name match only).
- This is a single self-contained HTML file with inlined parcel/ownership data; the aerial, street-label, and Sanborn layers load live from their respective free public services at view time.
