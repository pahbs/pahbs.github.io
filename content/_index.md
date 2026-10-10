---
date: "2022-10-24"
sections:
- block: about.biography
  content:
    title: 
    username: admin
  id: about
- block: experience
  id: engagement
  content:
    title: 'Service & Engagement'
    text: ''
    date_format: Jan 2006
    items:
    - company: NASA Arctic/Boreal Vulnerability Experiment
      company_logo: org-above
      company_url: "https://above.nasa.gov"
      date_end: ""
      date_start: "2019-01-01"
      description: |2-
          Responsibilities include:
          * funded Co-I
          * Vegetation Structure Working Group Lead
          * Vegetation Structure & Function Working Group Co-Lead
      location: arctic/sub-arctic
      title: Science Team Member
    - company: Oak Ridge National Laboratory DAAC
      company_logo: org-ornldaac
      company_url: "https://daac.ornl.gov/"
      date_end: ""
      date_start: "2021-01-01"
      description: serves in an advisory role as an earth science data user to the  NASAs Terrestrial Ecology Program's data repository
      title: User Working Group Member
    - company: NASA Multi-Mission Algorithm and Analysis Platform
      company_logo: org-maap
      company_url: "https://maap-project.org"
      date_end: ""
      date_start: "2018-01-01"
      description: advisory role as a funded Co-I to NASA MAAP
      title: User Working Group Member
    - company: NASA Surface Topography & Vegetation Working Group Member
      company_logo: org-stv
      company_url: "https://science.nasa.gov/earth-science/decadal-surveys/decadal-stv/"
      date_end: ""
      date_start: "2024-04-01"
      # TODO: update description of STV working group role
      description: ""
      title: Working Group Member
- block: collection
  content:
    count: 3
    filters:
      author: ""
      category: ""
      exclude_featured: false
      exclude_future: false
      exclude_past: false
      folders:
      - post
      publication_type: ""
      tag: ""
    offset: 0
    order: desc
    subtitle: ""
    text: ""
    title: Recent Posts
  design:
    columns: "3"
    view: compact
  id: posts
- block: markdown
  id: maps
  content:
    title: Interactive maps
    subtitle: ''
    text: |-
      Browser-based maps for reviewing results at scale. Click any feature or pixel to query values.

      ### Arctic & boreal mapping
      <span class="text-muted"><small>Updated Oct 10, 2026</small></span>

      Circumpolar forest structure products served from NASA MAAP as cloud-optimized GeoTIFFs through a dynamic tiler.

      * [**Boreal vegetation height, 2016–2025 (v3.1)**](https://pahbs.github.io/maap_tools/maps/Review_maps_v3.1_height_VHR.html): annual 30 m height, plus 2 m height from WorldView-2/3 stereo across Alaska
      * [**Boreal forest structure v3.1**](https://pahbs.github.io/maap_tools/maps/Review_maps_v3.1.html): aboveground biomass density and height
      * [**NDVI trends from HLS**](https://pahbs.github.io/maap_tools/maps/Review_maps_HLS_trends.html): per-pixel NDVI trend from Harmonized Landsat Sentinel-2 (Alaska)
      * [**Taiga–tundra ecotone**](https://pahbs.github.io/maap_tools/maps/Review_maps_TTE.html): forest structure patterns across the boreal–tundra transition
      * [**ICESat-2 ATL08 v6 vs v7**](https://pahbs.github.io/maap_tools/maps/atl08_v6v7_diff_map.html): differences between ATL08 data releases

      Code: [maap_tools](https://github.com/pahbs/maap_tools)

      ### Evaluation sites for commercial spaceborne imagery
      <span class="text-muted"><small>Updated Sep 24, 2026</small></span>

      Standardized areas of interest (AOIs) for evaluating commercial satellite imagery, each with a unique site name, precise bounds (GeoJSON), and site attributes.

      * [**CSDA Evaluation Sites**](https://pahbs.github.io/csda_summaries/notebooks/aoi_csda_sites_map.html): sites for subject-matter experts to reference when requesting imagery for NASA Commercial Smallsat Data Acquisition (CSDA) evaluations
      * [**SLI FUSION Evaluation Sites**](https://pahbs.github.io/csda_summaries/notebooks/aoi_eval_sites_map.html): a broader set of calibration/validation sites for radiometric and geometric evaluation work

      Code: [csda_summaries](https://github.com/pahbs/csda_summaries)
  design:
    columns: "1"
- block: portfolio
  id: projects
  content:
    title: Projects
    filters:
      folders:
      - project
    default_button_index: 0
    buttons:
    - name: All
      tag: '*'
  design:
    columns: "1"
    view: showcase
    flip_alt_rows: false
- block: markdown
  content:
    subtitle: "boreal forests"
    text: '{{< gallery album="kotuykan-river-siberia" >}}'
    title: Photos from the field — Kotuykan River, Siberia
  design:
    columns: "1"
- block: markdown
  content:
    subtitle: "boreal forests"
    text: '{{< gallery album="seward-peninsula-alaska" >}}'
    title: Photos from the field — Seward Peninsula, Alaska
  design:
    columns: "1"
- block: collection
  content:
    filters:
      featured_only: true
      folders:
      - publication
    title: Featured Publications
  design:
    columns: "2"
    view: card
  id: featured
- block: collection
  content:
    filters:
      exclude_featured: true
      folders:
      - publication
    text: |-
      {{% callout note %}}
      Quickly discover relevant content by [filtering publications](./publication/).
      {{% /callout %}}
    title: Recent Publications
  design:
    columns: "2"
    view: citation
- block: collection
  content:
    filters:
      folders:
      - event
    title: Recent & Upcoming Talks
  design:
    columns: "1"
    view: compact
  id: talks
- block: tag_cloud
  content:
    title: Popular Topics
  design:
    columns: "2"
- block: contact
  content:
    address:
      city: Greenbelt
      country: United States
      country_code: US
      postcode: "20771"
      region: MD
      street: 8800 Greenbelt Rd
    autolink: true
    contact_links:
    # - icon: twitter
    #   icon_pack: fab
    #   link: https://twitter.com/Twitter
    #   name: DM Me
    # - icon: skype
    #   icon_pack: fab
    #   link: skype:echo123?call
    #   name: Skype Me
    # - icon: video
    #   icon_pack: fas
    #   link: https://zoom.com
    #   name: Zoom Me
    coordinates:
      latitude: "38.999945266698305"
      longitude: "-76.85380920196566"
    directions: https://maps.app.goo.gl/rm62bZBoqrdpHdWR9
    email: paul.m.montesano@nasa.gov
    form:
      formspree:
        id: null
      netlify:
        captcha: false
      provider: netlify
    # office_hours:
    # - Monday 10:00 to 13:00
    # - Wednesday 09:00 to 10:00
    # phone: 888 888 88 88
    subtitle: null
    text: Requests, inquiries, and grievances.
    title: Contact
  design:
    columns: "2"
  id: contact
title: ""
type: landing
---
