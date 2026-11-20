---
title: "An Earth observation specifications dashboard for optical imaging constellations"
subtitle: "Compare the detail, footprint, bands, revisit and orbits of commercial and civil optical satellites in one place."
summary: "An interactive dashboard that puts the specifications of commercial and civil optical imaging constellations side by side."
date: "2026-11-19T00:00:00Z"
lastmod: "2026-11-19T00:00:00Z"
authors:
- admin
categories:
- CSDA
tags:
- commercial imagery
- evaluation
- optical sensors
- dashboards
featured: false
draft: false
image:
  caption: "Image footprint vs. detail: multispectral GSD against swath width for each constellation."
  focal_point: ""
  placement: 2
  preview_only: false
projects: []
---

Specifications for optical imaging satellites are scattered across vendor sheets, papers and websites, in different units and definitions. This dashboard gathers them into one database and draws it as linked views, filterable by sector and status.

**[Open the dashboard ↗](https://pahbs.github.io/csda_summaries/html/vendor_specs.html)**

- **Imaging specs**: ground sample distance against swath width; finer detail comes with a narrower footprint.
- **Spectral response**: each constellation's band response curves, visible to shortwave infrared and thermal infrared.
- **Coverage**: swaths at true ground scale over a chosen [evaluation site](/post/2026-09-24-evaluation-sites-commercial-imagery/).
- **Revisit**: estimated revisit at 0°, 40° and 60° latitude, from each constellation's orbit, swath and pointing.
- **Launches & orbits**: launch dates, orbit altitudes and satellite sizes over time.

The dashboard is a work in progress; the code is in [csda_summaries](https://github.com/pahbs/csda_summaries).
