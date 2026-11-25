---
title: "A map interpretation guide for the taiga-tundra ecotone forest pattern classes"
subtitle: "Choose a conceptual landscape, select a pixel, and see how tree cover and its abruptness, together, describe orest structure pattern."
summary: "An interactive guide to how the taiga-tundra ecotone (TTE) forest structure pattern map classifies each 30 m pixel from tree cover and its abruptness."
date: "2026-11-25T00:00:00Z"
lastmod: "2026-11-25T00:00:00Z"
authors:
- admin
categories:
- ABoVE
- MAAP
tags:
- taiga-tundra ecotone
- boreal
- tree cover
- maps
featured: false
draft: false
image:
  caption: "From the guide: a gradual treeline as tree cover (left) and the classes it produces (center), with the arithmetic for one selected pixel (right)."
  focal_point: ""
  placement: 2
  preview_only: false
projects: []
---

The taiga-tundra ecotone (TTE) map classifies the cold edge of the boreal forest by the *pattern* of its tree cover, not just the amount ([Montesano et al. 2020](https://doi.org/10.1088/1748-9326/abb2c7)). Each 30 m pixel gets a class from two numbers: its tree canopy cover, and its **abruptness**, which compares how fast cover changes around the pixel with how much cover it has.

Those classes are easy to state but harder to picture on a map, so I built a small interactive guide.

**[Open the TTE map interpretation guide ↗](https://pahbs.github.io/tte/docs/tte_interpretation_guide.html)**

## How this guide works

Our map describing the pattern and extent of the circumpolar taiga-tundra ecotone has a fairly unruly set of classes. To improve understanding of ecotone forest patterns and help with interpretation this interactive guide to the map's classification explains how various ecotone forest patterns are classified in our map. Choose one of nine conceptual ecotone landscapes (gradual and rapid treelines, sharp edges, tree islands, gaps in forest, thin lines of trees, a checkerboard, a lakeshore). Each one is drawn as a grid of tree cover pixels next to the forest structure pattern classes the map would give them. Select any pixel, or move with the arrow keys, to see:

- **Its four neighbors** and the rate of change in cover across them, computed like a terrain slope with cover in place of elevation.
- **Its abruptness**, `(rate − cover) / (rate + cover)`, from −1 (uniform) to +1 (abrupt), with every step of the arithmetic shown.
- **Its class**, placed on a small tree cover × abruptness chart of the 11 classes.

You can also change a pixel's cover, mark it as water, or paint on the grid to build your own landscape.

## What this guide reveals

In a gradual treeline, cover falls by the same 3 % per pixel, so the rate of change is nearly constant. The classes still change across it, because the cover that rate is compared with keeps shrinking: the same slope reads as *Open & Uniform* at 27 % cover and *Sparse & Diffuse-rapid* at 3 %.

![A row across the gradual treeline: tree cover bars with the class and abruptness of each pixel below.](transect.png "One row of the gradual treeline: the slope is constant, but abruptness climbs as cover falls.")

Tree islands, patches of trees in 1 % cover, show the opposite surprise: the pixel *with* the trees can be the most uniform one on the map. A lone 100 % pixel has matching neighbors left and right and up and down, so its rate of change is 0 and its abruptness is −1, the minimum. Its four side neighbors take the change instead, at +0.97, so the island appears as a plus sign of *Sparse & Abrupt* around an *Intermediate & Closed* center. The middle of a 3 × 3 patch is uniform for the same reason, and a 1 % pixel wedged between two dense pixels gets a high rate because dense cover sits on two of its sides.

![The tree islands landscape: patches of 20 to 100 % cover in 1 % cover, ringed by Sparse & Abrupt pixels in the class grid.](tree_islands.png "The tree islands landscape, with the lone 100 % pixel selected.")

## Where it fits

The guide sits alongside the code in the [tte](https://github.com/pahbs/tte) repository, which now reproduces the original Google Earth Engine TTE workflow in Python on NASA's [MAAP](https://maap-project.org/), and runs with any tree canopy cover raster as input.
