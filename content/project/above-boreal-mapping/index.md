---
title: ABoVE boreal forest structure mapping
summary: "Circumpolar 30 m maps of boreal forest height and aboveground biomass from ICESat-2 and Harmonized Landsat Sentinel-2, produced on NASA MAAP for the Arctic-Boreal Vulnerability Experiment."
date: "2026-10-10T00:00:00Z"
authors:
- admin
tags:
- ABoVE
- ICESat-2
- HLS
- MAAP
- boreal
- forest structure
image:
  caption: "v3.1 vegetation height for 2023 over North America, from the interactive map on the ESRI light gray basemap."
  focal_point: Smart
links:
- icon: map
  icon_pack: fas
  name: Interactive maps
  url: https://pahbs.github.io/maap_tools/maps/Review_maps_v3.1_height_VHR.html
- icon: database
  icon_pack: fas
  name: Dataset (ORNL DAAC)
  url: https://doi.org/10.3334/ORNLDAAC/2438
- icon: github
  icon_pack: fab
  name: icesat2_boreal
  url: https://github.com/lauraduncanson/icesat2_boreal
- icon: github
  icon_pack: fab
  name: maap_tools
  url: https://github.com/pahbs/maap_tools
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""
---

Part of the NASA [Arctic-Boreal Vulnerability Experiment (ABoVE)](https://above.nasa.gov), this project maps the structure of the circumpolar boreal forest at 30 m. It links ICESat-2 ATL08 lidar samples of vegetation height with Harmonized Landsat Sentinel-2 composites and Copernicus GLO-30 topography, using random forest models run tile by tile on NASA's [Multi-Mission Algorithm and Analysis Platform (MAAP)](https://maap-project.org).

The maps extend south to 51.6°N, the northern observational limit of NASA's GEDI mission, filling GEDI's northern data gap.

**Products**

- Vegetation height for 2020 ([ORNL DAAC dataset](https://doi.org/10.3334/ORNLDAAC/2438))
- Woody aboveground biomass for 2020 ([Duncanson et al. 2026](https://doi.org/10.1016/j.rse.2026.115406))
- An annual vegetation height time series for 2016–2025 (v3.1), in progress
- [Interactive maps](https://pahbs.github.io/maap_tools/maps/Review_maps_v3.1_height_VHR.html) for reviewing the products at scale
