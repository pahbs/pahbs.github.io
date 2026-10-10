---
title: "A decade of boreal vegetation height: the v3.1 2016–2025 time series"
subtitle: "An [**interactive map**](https://pahbs.github.io/maap_tools/maps/Review_maps_v3.1_height_VHR.html) of annual 30 m vegetation height across the circumpolar boreal, built on NASA MAAP."
summary: "Annual 30 m maps of boreal vegetation height for 2016–2025, from ICESat-2 and Harmonized Landsat Sentinel-2, in an interactive map you can explore year by year alongside 2 m height from very high resolution stereo imagery in Alaska."
date: "2026-10-10T00:00:00Z"
lastmod: "2026-10-10T00:00:00Z"
authors:
- admin
categories:
- MAAP
- ABoVE
tags:
- maps
- boreal
- ICESat-2
- HLS
- vegetation height
- time series
featured: true
draft: false
image:
  caption: "The interactive map zoomed to North America, showing v3.1 vegetation height for 2025 over the ESRI light gray basemap. Gaps are tiles still being processed for 2025."
  focal_point: ""
  placement: 2
  preview_only: false
projects: [above-boreal-mapping]
---

## Explore the map

**[Open the interactive map ↗](https://pahbs.github.io/maap_tools/maps/Review_maps_v3.1_height_VHR.html)**

The map shows two products on a shared 0–10 m color scale:

| Layer | Resolution | What it is |
|---|---|---|
| Vegetation height 2016–2025 (v3.1) | 30 m, annual | Vegetation canopy height modeled from ICESat-2 and Harmonized Landsat Sentinel-2 (HLS) |
| Vegetation height from WorldView-2/3 (c. 2018) | 2 m | Height from very high resolution stereo imagery across Alaska (zoom to level 3 or closer) |

Use the layer panel (top right) to switch years or basemaps, and click anywhere on the map to query pixel values.

## How the time series is made

Each annual layer comes from the same model, so differences between years reflect change in the inputs rather than changes in the model:

- **Training data**: ICESat-2 ATL08 (v6) canopy heights from 2019–2024, pooled across years.
- **Predictors**: an HLS composite for the target year, plus Copernicus GLO-30 topography.
- **Model**: random forest, fit repeatedly (30 iterations), giving a per-pixel mean height and a per-pixel standard deviation.
- **Processing**: tile by tile on NASA's [Multi-Mission Algorithm and Analysis Platform (MAAP)](https://maap-project.org), served as cloud-optimized GeoTIFFs through a dynamic tiler.

Because the same model is applied to each year's imagery, the series can be extended back to 2016, before ICESat-2 launched, and forward to 2025.

## Status

This is a work in progress. The 2019–2024 layers are nearly complete across the circumpolar domain. The 2016–2018 and 2025 layers cover a subset of tiles for now, which is why the 2025 view above is patchy. Those gaps are tiles still being processed, not missing forest.

Next up is validation against field plots and airborne lidar (LVIS and G-LiHT). It uses stand age to keep only the plots whose structure has not been altered by fire or harvest since they were measured.

## References

1. Montesano et al. (2026). ORNL DAAC. [doi:10.3334/ORNLDAAC/2438](https://doi.org/10.3334/ORNLDAAC/2438)
2. Montesano et al. (2026). *Environmental Research Letters*. [doi:10.1088/1748-9326/ae8e8f](https://doi.org/10.1088/1748-9326/ae8e8f)
3. Duncanson et al. (2026). *Remote Sensing of Environment*. [doi:10.1016/j.rse.2026.115406](https://doi.org/10.1016/j.rse.2026.115406)
4. Neuenschwander et al. (2024). *Science of Remote Sensing*. [doi:10.1016/j.srs.2024.100150](https://doi.org/10.1016/j.srs.2024.100150)
5. Frost et al. (2026). *IEEE International Geoscience and Remote Sensing Symposium (IGARSS)*. DOI pending.

Code: [maap_tools](https://github.com/pahbs/maap_tools) · [icesat2_boreal](https://github.com/lauraduncanson/icesat2_boreal)
