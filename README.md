# Iberian Energy Dashboard

Public dashboard of the Iberian electricity market (MIBEL): day-ahead prices for Portugal and
Spain, cross-border flows, renewable share, load-forecast accuracy and the platform's own data
quality. Live at https://kml0001gh.github.io/iberian-energy-dashboard/

This repository holds only the built site. It is published automatically by the CI of a private
data-engineering project (Python + dbt + Airflow lakehouse); the pages are static and read a small
extract of aggregated tables, never the raw data. Every page states the date the data is current to.

**Fonte/Source: OMIE, E-REDES (CC BY 4.0), IPMA, ENTSO-E Transparency Platform.**

Non-commercial portfolio project. Terms of the sources, as applied here:

- OMIE: day-ahead prices republished unmodified at their native resolution, source cited.
- E-REDES: CC BY 4.0.
- IPMA: free for non-commercial use, source cited.
- ENTSO-E Transparency Platform: actual load, generation per type and day-ahead prices appear only
  as derived daily aggregates; physical flows (12.1.G) are on the CC BY 4.0 free re-use list and
  are shown at native resolution. Modifications: omitted positions are forward-filled per
  ENTSO-E's curve type A03 and pivoted to one row per interval, and pre-October-2025 hourly prices
  are repeated per quarter-hour. See the About page for details.
