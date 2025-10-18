---
title: "Tools"
permalink: /tools/
layout: page
nav_key: tools

show_banner: true
banner_title: "echo-IA Tools"
banner_byline: "Software for IA research"
banner_cta: "Explore tools"
banner_cta_url: "/tools/"

hero:
  icon: "fa-solid fa-wrench"
  title: "echo-IA <strong>Tools</strong>"
  byline: "Software, scripts, and utilities supporting intrinsic alignment research."

blocks:
  # Overview
  - type: md
    title: "What you’ll find"
    content: |
      - **Core packages:** libraries for IA modeling, cosmology, and analysis.
      - **Workflows:** pipelines and reproducible analysis setups.
      - **Utilities:** plotting, diagnostics, and data preparation scripts.

      _Want to share your code? Use [Submit](/submit/) or [Contact](/contact/)._

  # Guides (unlisted)
  - type: buttons
    items:
      - label: "IA 101 — Practical steps"
        url: "/tools/ia-101/"

  # Featured tools (reads from _data/tools.yml; auto-hides if empty)
  - type: features
    title: "Featured"
    # no `items:` here — will read site.data.tools.featured

  # Categories
  - type: md
    title: "Categories"
    content: |
      #### Measurement
      - Shape and IA estimators, pseudo-Cℓ pipelines, null tests.

      #### Modeling
      - NLA, z-NLA, TATT, halo-model, and perturbative IA implementations.

      #### Pipelines
      - End-to-end or modular workflows from catalogs to posteriors.

      #### Utilities
      - Covariance calculators, QA diagnostics, and visualization helpers.

  # Contribute
  - type: md
    title: "Contribute your tool"
    content: |
      Add your IA-related package, notebook, or analysis helper to the list.
      Provide a short description, repository link, and documentation if available.

      - [Submit](/submit/)
      - [Contact](/contact/)
---
