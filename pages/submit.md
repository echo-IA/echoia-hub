---
title: "Submit"
permalink: /submit/
layout: page
nav_key: submit

show_banner: true
banner_title: "Submit your resource"
banner_byline: "Add shape catalogs, tools, notebooks, or datasets"
banner_cta: "Contact us"
banner_cta_url: "/contact/"

hero:
  icon: "fa-regular fa-square-plus"
  title: "Submit a Resource"
  byline: "Open a pre-filled GitHub issue. We’ll review and add it."

blocks:
  # Catalog submission form
  - type: issue_form
    preset: "submit_catalog"

  # Optional: Tool submission form
  - type: issue_form
    preset: "submit_tool"

  # Optional: Dataset submission form
  - type: issue_form
    preset: "submit_dataset"

  # (Optional) A compact help section
  - type: md
    title: "What happens next?"
    content: |
      - We’ll review your submission for completeness (license, link/DOI, minimal metadata).
      - If all good, we’ll add it to the site (and Zenodo collection when applicable).
      - We may comment on the GitHub issue if we need clarification.
---
