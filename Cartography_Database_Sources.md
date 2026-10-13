# Cartography Database Sources

## Satellite data, remote sensing and interactive environmental platforms

Version: 1.0  
Updated: 12 October 2026  
Project: ecological-information  
Purpose: a growing student reference for finding, viewing, analysing and reusing Earth-observation information.

This register consolidates 22 distinct resources discussed in the conversation. MapBiomas is listed once. It includes supporting computation and map-making tools as well as remote-sensing sources. Capability assessments are based on reviewed provider documentation, not an end-to-end test of every platform. Interfaces and access conditions can change.

## Capability definitions

- **View:** explore imagery or thematic maps in a browser.
- **Analyse:** perform comparisons, queries, statistics or calculations online. Limited includes inspection and predefined comparisons rather than arbitrary calculations.
- **Download:** obtain analytical pixel values or geographic features. Linked-service and product-dependent entries require checking the specific route or layer. Screenshots alone do not qualify.

## Source inventory

| ID | Resource | Information | View | Analyse | Download | Coverage | Access | Example exercise | Reuse / limitations |
|---|---|---|---|---|---|---|---|---|---|
| RS001 | [Copernicus Browser](https://browser.dataspace.copernicus.eu/) | Satellite imagery and indices | Yes | Yes | Yes | Global | Free account for analytical exports | Compare seasonal NDVI | GeoTIFF; raw versus rendered export matters |
| RS002 | [USGS EarthExplorer](https://earthexplorer.usgs.gov/) | Landsat reflectance and temperature | Yes | No | Yes | Global | Login for downloads | Investigate long-term landscape change | Follow product scaling and quality masks |
| RS003 | [NASA Worldview](https://worldview.earthdata.nasa.gov/) | Dated satellite and environmental layers | Yes | Limited | Linked service | Global | Browsing accessible; linked data access varies | Compare smoke or regional events | Snapshots are not necessarily analytical data |
| RS004 | [Copernicus Land Monitoring Service](https://land.copernicus.eu/en) | Land cover and environmental variables | Yes | Product-dependent | Yes | Global / Europe, by product | Product-dependent | Compare vegetation and developed land | Check resolution, period and product documentation |
| RS005 | [ESA WorldCover](https://viewer.esa-worldcover.org/) | 10 m land-cover maps: 2020 and 2021 | Yes | Limited | Yes | Global | Terrascope account for viewer downloads; alternatives exist | Map land-cover proportions | Algorithms differ between years; GeoTIFF and QGIS styles |
| RS006 | [Dynamic World](https://www.dynamicworld.app/) | 10 m land-cover classes and probabilities | Yes | Limited / Earth Engine | Via Earth Engine | Global, subject to observations | Earth Engine registration for custom exports | Examine classification uncertainty | Per-observation classification varies with conditions |
| RS007 | [Global Nature Watch map](https://globalnaturewatch.org/map/) | Forest and ecosystem change and alerts | Yes | Yes | Layer-dependent | Layer-dependent | Check layer access | Investigate tree-cover loss | Tree-cover loss is not automatically deforestation |
| RS008 | [Global Nature Watch Horizon](https://horizon.globalnaturewatch.org/) | AI-assisted environmental queries | Yes | Yes | Source-dependent | Dataset-dependent | Preview platform | Formulate and verify landscape questions | Verify AI summaries and source datasets |
| RS009 | [MapBiomas](https://mapbiomas.org/) | Annual land-cover and land-use maps | Yes | Yes | Yes | Participating countries / regions | Regional platform requirements vary | Study agricultural expansion | Coverage, collections and methods vary |
| RS010 | [Resource Watch](https://resourcewatch.org/) | Environmental and social layers | Yes | Limited | Yes / source-dependent | Dataset-dependent | Dataset-dependent | Overlay human and ecological conditions | Preserve original dataset attribution |
| RS011 | [Global Mangrove Watch](https://www.globalmangrovewatch.org/) | Mangrove extent, change and alerts | Yes | Yes | Layer-dependent | Mangrove regions globally | Check selected layer | Compare coastal ecosystem change | Check indicator applicability at local scale |
| RS012 | [Allen Coral Atlas](https://allencoralatlas.org/) | Coral-reef habitat maps and monitoring | Yes | Limited | Yes | Mapped coral-reef regions | Follow download instructions | Explore reef habitat distribution | Attribution required; coverage and depth limits |
| RS013 | [JRC Global Surface Water](https://global-surface-water.appspot.com/) | Water occurrence, seasonality and change | Yes | Limited | Yes | Global | Free tile downloads | Study reservoir water persistence | GeoTIFF; custom analysis in GIS or Earth Engine; check release notes |
| RS014 | [GloFAS / Global Flood Monitoring](https://global-flood.emergency.copernicus.eu/) | Flood forecasts and satellite inundation | Yes | Limited | Product-dependent | Global, product-dependent | Account and product-specific access | Compare forecasts with observed inundation | Forecasts and satellite observations are distinct |
| RS015 | [Copernicus Drought Observatories](https://drought.emergency.copernicus.eu/) | European and global drought indicators | Yes | Yes | Yes | Europe / Global | Check selected indicator | Compare drought periods in Catalonia | Includes satellite, meteorological and model inputs |
| RS016 | [EFFIS](https://forest-fire.emergency.copernicus.eu/) | Fires, burned areas, danger and risk | Yes | Yes | Product-dependent | Europe and neighbouring regions | Services or data requests vary | Study Mediterranean fire events | Separate detected events, burned area and forecast danger |
| RS017 | [NASA FIRMS](https://firms.modaps.eosdis.nasa.gov/) | Active fires and thermal anomalies | Yes | Limited | Yes | Global | Archive authentication; recent downloads available | Map thermal detections | CSV/KML/shapefile; hotspots are not burn boundaries |
| RS018 | [Copernicus Marine MyOcean Pro](https://data.marine.copernicus.eu/viewer/expert) | Marine observations and models | Yes | Yes | Yes | Global / regional products | Download requirements vary | Plot marine change through time | Commonly NetCDF; distinguish model from observation |
| RS019 | [Global Human Settlement Layer](https://human-settlement.emergency.copernicus.eu/) | Built-up areas, settlements and population | Yes | Limited | Yes | Global | Open downloadable products | Investigate urbanisation | Population is estimated; check product resolution |
| RS020 | [Google Earth Engine](https://code.earthengine.google.com/) | Scripted geospatial computation | Yes | Yes | Yes | Dataset-dependent | Registered Cloud project; noncommercial eligibility verification | Calculate composites and zonal statistics | Coding and export limits; dataset-specific licences |
| RS021 | [ICGC viewers and downloads](https://www.icgc.cat/en/Tools-and-viewers/Viewers) | Orthophotos, LiDAR and cartography | Yes | Limited | Yes | Catalonia | Product-dependent | Inspect terraces and local terrain | Includes airborne rather than satellite sensing |
| RS022 | [Instamaps](https://www.instamaps.cat/) | Create and share personalised maps | Yes | Limited | Layer-dependent | User-data / basemap-dependent | Check publishing/account requirements | Present annotated student maps | Map presentation tool, not a satellite processing engine |

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

## Student starting sequence

1. Copernicus Browser: inspect one place in natural colour, infrared and NDVI.
2. WorldCover: compare observed patterns with classified land cover.
3. Global Surface Water: examine water persistence and seasonality.
4. Drought Observatories or EFFIS: investigate a relevant environmental pressure.
5. Global Nature Watch: investigate ecosystem change and alerts.
6. Instamaps or QGIS: communicate findings with source attribution.

## Interpretation and reuse

Download numerical data when calculations are needed; a GeoTIFF can also contain only rendered colours. WMS/WMTS commonly supply display images. Record dates, native resolution and processing choices. NDVI alone does not establish ecological health. WorldCover 2020 and 2021 use different algorithms. Fire hotspots do not delineate burned area. Forecasts, modelled estimates and AI summaries must be distinguished from observations.

## Version history

- 1.0 — Consolidated the original and additional resources; introduced stable source IDs, View / Analyse / Download capabilities and a dataset metadata schema.

