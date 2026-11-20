---
title: "An Earth observation specifications dashboard for optical imaging constellations"
subtitle: "One place to compare the detail, footprint, spectral bands, revisit and orbits of commercial and civil optical satellites."
summary: "An interactive dashboard that puts the specifications of about 40 commercial and civil optical imaging constellations side by side: resolution against swath, spectral response curves, swaths at true scale over evaluation sites, estimated revisit, launches and orbits, and a check on the database behind it all."
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
  caption: "Image footprint vs. detail: each constellation's multispectral ground sample distance against its swath width. Dashed lines count the pixels across the swath."
  focal_point: ""
  placement: 2
  preview_only: false
projects: []
---

Choosing commercial satellite imagery for a study, or evaluating it, starts with a set of questions about each sensor: how fine is the detail, how wide is the footprint, which bands does it carry, how often can it see a place, and how old and how high is the satellite? The answers are scattered across vendor sheets, papers and websites, in different units and with different definitions.

**[Open the dashboard ↗](https://pahbs.github.io/csda_summaries/html/vendor_specs.html)**

The Earth Observation Specifications Dashboard gathers them into one database of optical imaging constellations, commercial and civil, and draws it as a set of linked views. Filters for sector (commercial or civil) and status apply across all of them, any data owner can be highlighted, and **Find** narrows every view to a few named constellations for a direct comparison.

## What it shows

- **Imaging specs**: multispectral ground sample distance (GSD) against swath width, both on log scales. Dashed lines count the pixels across the swath: most sensors sit between about 3,000 and 30,000, so finer detail comes with a narrower footprint. A companion panel lines up the key specs one row per constellation, with multispectral and panchromatic GSD side by side.
- **Spectral response**: the relative spectral response curves of each constellation's bands on a shared wavelength axis, visible to shortwave infrared, and a separate chart for thermal infrared (mid-wave, water vapor, long-wave and CO₂ bands, in micrometres). Tables give each band's center (the response-weighted mean wavelength) and width at half the peak. Civil reference curves come from Pyspectral (MODIS, VIIRS, Sentinel-3) and GFZ pyrsr (Landsat 5 and 7); hyperspectral bands without measured curves are drawn from the vendor's band centers and widths and marked as modeled.
- **Coverage**: every constellation's swath drawn as a square at true ground scale, centered on a chosen site from the [evaluation sites database](/post/2026-09-24-evaluation-sites-commercial-imagery/), so the footprint of a single scene can be judged against the area it needs to cover.
- **Revisit**: estimated revisit time at 0°, 40° and 60° latitude, by view angle and season, from each constellation's orbit, swath and number of satellites. The assumptions behind the estimates are listed with the chart, most significant first.
- **Launches & orbits**: one mark per sensor at its launch date and orbit altitude, shaped by orbit type and sized by satellite class, with a line running to its end date or to today while it operates; planned missions are shown open.
- **Data table**: the constellations matching the filters, with the plotted values, sortable by any column.
- **Database quality**: how complete the database is (the share of sensors with each core field filled), automated consistency checks that flag suspect values, and the record of every edit made to it.

## Why a database, not a table

The specifications change: new satellites launch, vendors revise their numbers, and errors turn up when the data are put to use. Keeping them in one database, with automated checks and an edit record, makes each correction visible and traceable, and the dashboard is rebuilt from the database whenever it changes. Values still being confirmed are flagged on the charts rather than hidden.

## Status

The dashboard is a work in progress: constellations and spectral response curves are added as they become available, and values are checked against vendor documentation as evaluations proceed. The code is in [csda_summaries](https://github.com/pahbs/csda_summaries).
