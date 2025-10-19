---
title: "Home"
permalink: /
layout: page
nav_key: home

# Banner
show_banner: true
banner_title: "echo-IA"
banner_byline: "COLLABORATION"
banner_logo: /images/logos/echoia_logo_white_notext_transparent.svg
banner_logo_alt: "echo-IA logo"
banner_cta: "Tell me more"
banner_cta_url: "#home-top"

# Page blocks
blocks:
  - type: md
    anchor_id: "about"   # so the banner CTA "#about" scrolls here
    title: "About echo-IA"
    align: center
    content: |
      <a id="home-top"></a>
      echo-IA (Enabling Cosmology with Homogenized Observations of Intrinsic Alignments) is a community space for
      _intrinsic alignment_ research. We bring together catalogs, tools, datasets, and workflows so results are easier
      to compare, reproduce, and extend.

  - type: buttons
    align: center
    button_size: md
    items:
      - label: "About echo-IA"
        url: "/about/"
        size: lg
      - label: "Browse Tools"
        url: "/tools/"
        size: lg
      - label: "Workshops & Meetings"
        url: "/meetings/"
        size: lg
      - label: "Browse Catalogs"
        url: "/catalogs/"
        size: lg
---
