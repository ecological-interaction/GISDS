# GISDS

GIS and Remote Sensing Database Sources is an independent catalogue within the Ecological Information domain of Ecological Interaction. It is a reference for anyone finding, viewing, analysing or reusing GIS, cartography and Earth-observation information.

Catalogue version: 1.4  
Updated: 14 October 2026  
Status: Markdown catalogue; database implementation and integrations remain future work.

## Catalogue

Read [GISDS.md](GISDS.md), the current register of 25 resources with stable source IDs RS001–RS025. It includes data providers, environmental platforms, geospatial computation services and map-making tools. MapBiomas is listed once. The seven descriptive columns cover ID, resource, information available, coverage, accessibility, example use and reuse / limitations.

GISDS.md contains only the source table. This README holds purpose, guidance, metadata conventions, provenance and version history. [Cartography_Database_Sources.md](Cartography_Database_Sources.md) is the preserved original catalogue and has not been updated by this revision.

Descriptions are based on reviewed provider documentation, not an end-to-end test of every platform. Interfaces and access conditions can change. No software installation is required to read the catalogue. Follow each provider's access, attribution and reuse requirements and record the checked date when reviewing an entry.

## Dataset-level fields

Create a separate record for each dataset actually used. A platform may host many products with different characteristics.

| Field | Required content |
|---|---|
| Dataset ID | Stable identifier linked to the source ID above |
| Product / layer | Exact dataset name and version |
| Observation type | Satellite, airborne, derived classification, model or combined indicator |
| Geographic coverage | Extent and coverage gaps |
| Acquisition / reference period | Actual date or period represented |
| Update frequency | Release or observation interval |
| Spatial resolution | Native pixel size or mapping scale |
| Download format | GeoTIFF, CSV, GeoPackage, shapefile, NetCDF or other |
| CRS | Coordinate reference system |
| Processing | Masks, scaling, indices, resampling and other transformations |
| Account / cost | Access requirements and limits |
| Licence / attribution | Dataset-specific reuse conditions and citation |
| Download URL | Product-specific route rather than only platform homepage |
| Checked date | Date access and documentation were last reviewed |
| Limitations | Clouds, uncertainty, gaps, algorithm changes and comparability |
| Boundary applications | Catchment, classified land-cover patch, terrain transition or visually interpreted land-use boundary |
| Local-scale suitability | Native resolution or mapping scale and suitability for the selected study area |

## Suggested starting sequence

1. Copernicus Browser: inspect one place in natural colour, infrared and NDVI.
2. WorldCover: compare observed patterns with classified land cover.
3. Global Surface Water: examine water persistence and seasonality.
4. Drought Observatories or EFFIS: investigate a relevant environmental pressure.
5. Global Nature Watch: investigate ecosystem change and alerts.
6. Instamaps or QGIS: communicate findings with source attribution.

## Interpretation and reuse

Download numerical data when calculations are needed; a GeoTIFF can also contain only rendered colours. WMS/WMTS commonly supply display images. Record dates, native resolution and processing choices. NDVI alone does not establish ecological health. WorldCover 2020 and 2021 use different algorithms. Fire hotspots do not delineate burned area. Forecasts, modelled estimates and AI summaries must be distinguished from observations.

## Local boundary work and review provenance

For a local exercise, compare orthophotos, a numerical terrain model and classified land cover. A tree-cover class boundary is not a complete ecological boundary. Delineate catchments using terrain extending beyond the final presentation area, then crop the output. Keep imagery, LiDAR and elevation products as separate dataset records linked to RS021 or RS025; the links above do not constitute completed dataset records. Enter the exact version, acquisition dates, resolution, CRS, processing and licence when selecting data.

Revision basis: the final entry in **GISDS Overview**, 14 October 2026, the revised `Cartography_Database_Sources.md` v1.1, and the existing `GISDS.md` v1.2. RS001–RS024 retain their identifiers; ICGC links extend RS021 rather than duplicate it.

Provider review on 14 October 2026: [ICGC elevation documentation](https://www.icgc.cat/ca/Geoinformacio-i-mapes/Dades-i-productes/Elevacions/Elevacions-territorial/Models-delevacions) and [download selector](https://visors.icgc.cat/appdownloads/) support the revised RS021 entry. [IGN PNOA documentation](https://pnoa.ign.es/pnoa-lidar/productos-a-descarga) supports RS025. The CNIG homepage returned a fetch error and VISSIR supplied no extractable text; their interactive workflows were not tested. Other entries retain the prior reviewed register descriptions and were not reverified for this revision.

## Version history

- 1.4 — Kept GISDS.md as one continuous source table, joined RS025 to the other rows, changed the use column and entry wording for a general audience, and moved supporting guidance and version history to README.md. Updated AGENTS.md to maintain this structure.

- 1.3 — Added CNIG/IGN as RS025, expanded RS021 with specific ICGC viewer and product links, added boundary metadata guidance and recorded review provenance; retained descriptive columns and RS001–RS024. Saved as GISDS.md in the GISDS folder.

- 1.2 — Renamed the document GISDS.md and updated its title; retained the GISDS Overview changes and joined all 24 sources into one continuous table.

- 1.1 — Restored descriptive source-list columns; removed View / Analyse / Download columns and capability definitions; added AlphaEarth Foundations (RS023) and Google Earth AI (RS024). Existing source IDs retained.

- 1.0 — Consolidated the original and additional resources; introduced stable source IDs, View / Analyse / Download capabilities and a dataset metadata schema.


## Related projects

GISDS complements EII's ecological indicator inventory, EIRKB's research and reference architecture, and AMRKB's agricultural knowledge. It remains independently maintained; shared identifiers, provenance and metadata conventions can support later interoperability without a shared runtime dependency.

## Maintenance

Keep source IDs and filenames stable. Retain attribution and provenance, and distinguish documented capabilities from untested assumptions. Record catalogue versions, dates and review history here. Licensing and repository citation metadata have not yet been selected; dataset reuse conditions remain those of their respective providers.
