---
title: "Two maps of evaluation sites for commercial spaceborne imagery"
subtitle: "Standardized areas of interest for evaluating commercial satellite data: the CSDA and SLI FUSION evaluation site databases."
summary: "Two interactive maps of standardized evaluation sites, one for requesting commercial imagery for NASA CSDA evaluations and a broader one for SLI FUSION calibration/validation work, so evaluators share the same site names and boundaries."
date: "2026-09-24T00:00:00Z"
lastmod: "2026-09-24T00:00:00Z"
authors:
- admin
categories:
- CSDA
tags:
- commercial imagery
- evaluation
- calibration/validation
- maps
featured: false
draft: false
image:
  caption: "The SLI FUSION Evaluation Sites map: AOIs colored by the source of each site."
  focal_point: ""
  placement: 2
  preview_only: false
projects: []
---

Evaluating commercial satellite imagery depends on comparing it, again and again, against well-characterized places on the ground. These two maps make those places easy to find and reference. Every area of interest (AOI) has:

- a unique **site name**,
- precise **boundaries** stored in a GeoJSON file, and
- **attributes** describing the site: the subject-matter domain (e.g., optical multispectral/hyperspectral, thermal IR, SAR, DEM), the evaluation category (radiometric or geometric), and the source of the site.

On both maps, AOIs are drawn with a 25 km vicinity buffer so they stay visible at global scale, and are colored by their source. Click any site for its details.

## CSDA Evaluation Sites

**[Open the map ↗](https://pahbs.github.io/csda_summaries/notebooks/aoi_csda_sites_map.html)**

A standardized set of locations for subject-matter experts to reference when submitting imagery requests for NASA Commercial Smallsat Data Acquisition (CSDA) evaluations. Using a shared site name and boundary in every request means imagery from different vendors, sensors and dates can be compared over exactly the same ground. The map holds about 240 AOIs, drawn from NASA, JPL, ESA, DLR, KIT, RadCalNet, USGS and USGS 3DEP sites.

## SLI FUSION Evaluation Sites

**[Open the map ↗](https://pahbs.github.io/csda_summaries/notebooks/aoi_eval_sites_map.html)**

A broader database of about 600 AOIs for calibration/validation and other evaluation work. Alongside most of the CSDA sites, it adds established reference networks, mostly for radiometric evaluation:

- AERONET and AERONET-OC
- BELMANIP2
- the National Data Buoy System
- SkyCam and HyperNAV
- NEON (including sites for geolocation assessment)
- USDA

Bringing these networks into one map, with the same naming and attributes, makes it quicker to find a suitable reference site for a given sensor and evaluation type.

## Status

Both databases are works in progress: AOIs are being added and adjusted as evaluations proceed. The code and site files are in [csda_summaries](https://github.com/pahbs/csda_summaries).
