---
title: "Resolving Alaska's boreal-tundra with 2 m vegetation height"
subtitle: "New in *Environmental Research Letters*: a foundation model fine-tuned on commercial imagery maps short-statured shrubs and trees across the biome boundary."
summary: "We fine-tuned a vision foundation model with commercial very high resolution imagery and airborne height data to map vegetation height at 2 m across 40% of Alaska's boreal-tundra ecotone. Most of this landscape is under 1.5 m tall, and the height classes separate low shrubs, tall shrubs, and forest."
date: "2026-08-04T00:00:00Z"
lastmod: "2026-08-04T00:00:00Z"
authors:
- admin
categories:
- VHR
- ABoVE
tags:
- VHR
- vegetation height
- foundation model
- boreal-tundra ecotone
- Alaska
- shrubs
featured: false
draft: false
image:
  caption: "Figure 3 from Montesano et al. (2026), *Environmental Research Letters*, CC BY 4.0."
  focal_point: ""
  placement: 2
  preview_only: false
projects: []
---

**Paper:** Montesano, P. M., Frost, M., Caraballo-Vega, J. A., Macander, M. J., Frost, G. V., Neigh, C. S. R., Fried, N. A., Spradlin, C., Mannix, J., & Carroll, M. (2026). Alaska's boreal-tundra resolved with vegetation height from commercial imagery and a foundation model. *Environmental Research Letters*, 21, 154021. [doi:10.1088/1748-9326/ae8e8f](https://doi.org/10.1088/1748-9326/ae8e8f) (open access)

## Why it matters

Vegetation structure in the boreal forest–tundra ecotone and the Low Arctic is shifting with shrub expansion, tree advance, permafrost thaw, and disturbance. Most of this vegetation is short, so even very high resolution (VHR) satellite imagery and Earth-observation AI models have struggled to separate one plant functional type from another by height.

## What we did

- **Imagery**: a large archive of commercial VHR imagery from July–August, standardized to surface reflectance so that imagery from many acquisitions can be used together ([see our surface reflectance workflow](/publication/surface-reflectance-from-vhr/)).
- **Model**: we fine-tuned the DINOv3 vision foundation model to predict vegetation height. Training used canopy height models from airborne lidar and airborne IFSAR across Alaska.
- **Validation**:
  - an extensive comparison with NASA LVIS airborne lidar, totaling more than 84 million 10 m observations;
  - an intensive comparison with field transects and UAV surveys from an August 2024 campaign on the Seward Peninsula.

## What we found

Across about 40% of Alaska's boreal-tundra ecotone, mapped at 2 m:

- **63.4% ± 5.2%** of the area is low-stature vegetation under 0.35 m.
- **Low shrubs** (0.35–1.5 m) cover about 18% (11.9% ± 1.2% and 6.3% ± 1.1%).
- **Tall shrubs and forest** (≥ 1.5 m) make up the remaining ~18%.
- Altogether, about 82% of the mapped landscape is under 1.5 m tall.

Predictions underestimate the very tops of canopies. They agree best with the 75th–85th percentile lidar heights rather than the 98th.

## Explore and reuse

- The 2 m heights are a layer in the [interactive boreal vegetation height map](https://pahbs.github.io/maap_tools/maps/Review_maps_v3.1_height_VHR.html) ("Vegetation height from VHR"). Zoom to level 3 or closer over Alaska.
- Code and data: [github.com/nasa-nccs-hpda/above-shrubs](https://github.com/nasa-nccs-hpda/above-shrubs)

This work was supported by the NASA Arctic-Boreal Vulnerability Experiment (ABoVE).
