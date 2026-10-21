# GISDS

**Work in Progress — Academic Research Resource**

Research by Jonathan Minchin, Ecological Interaction.
[ORCID 0000-0001-8152-1796](https://orcid.org/0000-0001-8152-1796).
See [CITATION.cff](CITATION.cff) for academic attribution and
[CHANGELOG.md](CHANGELOG.md) for publication-preparation history.

GIS and Remote Sensing Database Sources is an independent catalogue within the Ecological Information domain of Ecological Interaction. It is a reference for anyone finding, viewing, analysing or reusing GIS, cartography and Earth-observation information.

Catalogue version: 1.4  
Updated: 14 October 2026  
Status: Markdown catalogue; database implementation and integrations remain future work.

## Catalogue

Read [GISDS.md](GISDS.md), the current register of 25 resources with stable source IDs RS001–RS025. It includes data providers, environmental platforms, geospatial computation services and map-making tools. MapBiomas is listed once. The seven descriptive columns cover ID, resource, information available, coverage, accessibility, example use and reuse / limitations.

GISDS.md contains only the source table. This README holds purpose, guidance, metadata conventions, provenance and version history. The original `Cartography_Database_Sources.md` is preserved in Git commit `1469382a8bab95cf277c2a8c3996c949351a40ad`; it is not present in the current working tree. Its historical content remains unchanged.

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

No licence has been selected for this repository or its research documentation.
Public accessibility does not itself grant permission to reuse, redistribute or
adapt this material. Citation metadata provides attribution information, not a
licence. Third-party resources and datasets retain their own licences, access
conditions and attribution requirements; inclusion in GISDS grants no additional
reuse permissions.

Download numerical data when calculations are needed; a GeoTIFF can also contain only rendered colours. WMS/WMTS commonly supply display images. Record dates, native resolution and processing choices. NDVI alone does not establish ecological health. WorldCover 2020 and 2021 use different algorithms. Fire hotspots do not delineate burned area. Forecasts, modelled estimates and AI summaries must be distinguished from observations.

## Local boundary work and review provenance

For a local exercise, compare orthophotos, a numerical terrain model and classified land cover. A tree-cover class boundary is not a complete ecological boundary. Delineate catchments using terrain extending beyond the final presentation area, then crop the output. Keep imagery, LiDAR and elevation products as separate dataset records linked to RS021 or RS025; the links above do not constitute completed dataset records. Enter the exact version, acquisition dates, resolution, CRS, processing and licence when selecting data.

Revision basis: the catalogue review of 14 October 2026, the revised `Cartography_Database_Sources.md` v1.1, and the existing `GISDS.md` v1.2. RS001–RS024 retain their identifiers; ICGC links extend RS021 rather than duplicate it.

Provider review on 14 October 2026: [ICGC elevation documentation](https://www.icgc.cat/ca/Geoinformacio-i-mapes/Dades-i-productes/Elevacions/Elevacions-territorial/Models-delevacions) and [download selector](https://visors.icgc.cat/appdownloads/) support the revised RS021 entry. [IGN PNOA documentation](https://pnoa.ign.es/pnoa-lidar/productos-a-descarga) supports RS025. The CNIG homepage returned a fetch error and VISSIR supplied no extractable text; their interactive workflows were not tested. Other entries retain the prior reviewed register descriptions and were not reverified for this revision.

## Version history

- 1.4 — Kept GISDS.md as one continuous source table, joined RS025 to the other rows, changed the use column and entry wording for a general audience, and moved supporting guidance and version history to README.md. Updated AGENTS.md to maintain this structure.

- 1.3 — Added CNIG/IGN as RS025, expanded RS021 with specific ICGC viewer and product links, added boundary metadata guidance and recorded review provenance; retained descriptive columns and RS001–RS024. Saved as GISDS.md in the GISDS folder.

- 1.2 — Renamed the document GISDS.md and updated its title; retained the preceding catalogue revisions and joined all 24 sources into one continuous table.

- 1.1 — Restored descriptive source-list columns; removed View / Analyse / Download columns and capability definitions; added AlphaEarth Foundations (RS023) and Google Earth AI (RS024). Existing source IDs retained.

- 1.0 — Consolidated the original and additional resources; introduced stable source IDs, View / Analyse / Download capabilities and a dataset metadata schema.


## Related projects

GISDS complements EII's ecological indicator inventory, EIRKB's research and reference architecture, and AMRKB's agricultural knowledge. It remains independently maintained; shared identifiers, provenance and metadata conventions can support later interoperability without a shared runtime dependency.

## Maintenance

Keep source IDs and filenames stable. Retain attribution and provenance, and distinguish documented capabilities from untested assumptions. Record catalogue versions, dates and review history here. Citation metadata is provided in `CITATION.cff`. No repository licence has been selected; dataset reuse conditions remain those of their respective providers.

## Publication preparation

The configured Git remote is
[Jonathan-Minchin/GISDS](https://github.com/Jonathan-Minchin/GISDS).
On 21 October 2026, both this location and the potential organisation location
`ecological-interaction/GISDS` returned HTTP 404 to anonymous requests. Public
access and ownership transfer are therefore unverified; the remote has not
been changed. Author affiliation with Ecological Interaction does not imply
that the organisation owns or publicly hosts this repository.

The proposed academic reading interface is `/information/GISDS/` on the
Ecological Interaction website. It is not integrated or published by this
preparation. `GISDS.md` should supply the resource catalogue, with this README
providing scope, interpretation, dataset metadata guidance and provenance.
Approved versions can later be imported by full Git commit and SHA-256
checksums, without maintaining independent academic copies in the website.
No downloadable dataset is included in this repository.

Read-only link checks on 21 October 2026 reached 29 of the 30 distinct provider
URLs; the ESA WorldCover viewer returned HTTP 403 and needs browser review.
Google Earth Engine redirected to sign-in. Successful HTTP responses establish
reachability only, not scientific verification, access rights or successful
interactive downloads. The earlier dated provider-review findings above
remain historical observations and have not been replaced with new capability
claims.
