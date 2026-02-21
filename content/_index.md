---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/resume.pdf
    design:
      css_class: dark
      background:
        color: black
        image:
          # Add your image background to `assets/media/`.
          filename: drbg2.svg
          filters:
            brightness: 0.5
          size: cover
          position: center
          parallax: false
  - block: markdown
    content:
      title: '📊 Decision Science & Analytics'
      subtitle: ''
      text: |-
        Dr. Md Marufur Rahman is a healthcare decision scientist and physician-researcher with over 10 years of experience translating complex health data into evidence-based recommendations for senior decision-makers. Currently serving as **Senior Performance Measurement Specialist** at the Saskatchewan Ministry of Health, he reviews analytical outputs, critically appraises data visualizations, and prepares data-backed policy recommendations across Continuing Care, Mental Health & Addictions, and Acute Care programs.

        His expertise spans **predictive modelling, statistical inference, machine learning**, and health system performance measurement. He holds a PhD in Medicine from the University of Sheffield, where he applied deep learning and multivariate statistical methods to clinical oncology data. He has led national-scale health information systems in collaboration with WHO, UNICEF, and UNDP, and brings direct experience with MoH–SHA Performance Agreements, CIHI indicators, and Saskatchewan's health system priorities.

        He is also an advocate for science communication and AI innovation in public health — building custom agentic AI systems using Microsoft Copilot Studio and the Claude API to enhance healthcare analytics capacity.
    design:
      columns: '1'
  - block: collection
    id: papers
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      view: article-grid
      columns: 2
  - block: collection
    content:
      title: All Publications & Reports
      text: ""
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: citation
---
