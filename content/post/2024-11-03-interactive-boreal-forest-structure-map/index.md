---
authors:
- admin
categories:
- MAAP
- ABoVE
date: "2024-11-03T00:00:00Z"
draft: false
featured: false
image:
  caption: Screenshot of the folium map displaying COGs of AGB predictions at 30m resolution hosted on MAAP.
  focal_point: ""
  placement: 2
  preview_only: false
lastmod: "2024-11-03T00:00:00Z"
projects: [Mapping]
subtitle: A rendered `Jupyter` notebook with an [**interactive map**](https://notebooksharing.space/view/68349c623d52dea574975392ac86b9772c2f375f7883d33bf8a4865b9b9e6f46#displayOptions=hide-inputs).
summary: "Here we share a jupyter notebook running folium and a dynamic raster tiler to display an interactive map of our 2020 boreal aboveground biomass density and forest height estimates. We use this to visually review our results at scale."
tags:
- maps
- boreal
- folium
title: Interactive map of 30m boreal forest aboveground biomass and height
---

## Review 30m raster predictions of boreal forest structure with dynamic tiling

Here we share a `Jupyter` notebook running `folium` and a dynamic raster tiler called `TiTiler` to display thousands of cloud-optimized geotiffs (COGs) in an interactive map built on NASA's Multi-Mission Algorithm and Analysis Platfor ([**MAAP**](https://maap-project.org/)).

This map features 2 layers that are the result of empirical model predictions of forest structure at 30 m resolution across the full circumpolar domain for year `2020`:

-   boreal aboveground biomass density [Mg/ha]\
-   boreal vegetation height [m]
