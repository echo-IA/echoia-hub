---
title: "Catalogs"
permalink: /catalogs/
layout: page
nav_key: catalogs

# Top banner
show_banner: true
banner_title: "Shape Catalogs"
banner_byline: "echo-IA Community"
banner_cta: "Submit a catalog"
banner_cta_url: "/submit/"

# Load PapaParse on this page (your scripts include looks for this)
papaparse: true

# Page hero (replaces the old `{% include hero.html ... %}`)
hero:
  icon: "fa-regular fa-table"
  title: "Browse <strong>shape catalogs</strong>"
  blurb: "Find public galaxy shape catalogs with consistent high-level metadata, licensing notes, and links to their original hosts."

blocks:
  # Data-driven expandable list (reuses your existing catalogs_list.html)
  - type: catalogs_list
    data_key: "catalogs"

  # Three-up feature row
  - type: feature_row
    items:
      - title: "Contribute"
        text: "Submit a new catalog with DOI, license, and minimal metadata."
        button_label: "Submit"
        url: "/submit/"
      - title: "Licensing"
        text: "We list license info; datasets remain © their owners at the original host."
        button_label: "Learn More"
        url: "/catalogs/#license"
      - title: "Roadmap"
        text: "Toward a unified IA pipeline built on shared, comparable inputs."
        button_label: "Open Issues"
        url: "https://github.com/echo-IA/echoia-hub/issues"
---
