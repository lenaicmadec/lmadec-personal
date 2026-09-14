---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2022-10-24
type: landing

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: me
      text: ''
      # Show a call-to-action button under your biography? (optional)
      #button:
      #  text: Download CV
      #  url: uploads/resume.pdf
      headings:
        about: ''
        education: ''
        interests: ''
    design:
      # Use the new Gradient Mesh which automatically adapts to the selected theme colors
      background:
        gradient_mesh:
          enable: true

      # Name heading sizing to accommodate long or short names
      name:
        size: md # Options: xs, sm, md, lg (default), xl

      # Avatar customization
      avatar:
        size: medium # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded
  - block: markdown
    content:
      title: '💡 My Research'
      subtitle: ''
      text: |-
        My research activity lies between the fundamental and applied fields with a focus on interfacial phenomena that govern the M-ion and solid-state batteries performance. In particular, I developed innovative cross-section preparation and *in situ/operando* analysis to study the buried interfaces of solid-state batteries. I also developed an approach to combine XPS with GC/MS/FTIR to further understand parasitic reaction at the interfaces of M-ion batteries with an emphasis on the emerging K-ion batteries.
    design:
      columns: '1'
  - block: collection
    id: papers
    content:
      title: Featured Publications
      filters:
        folders:
          - publications
        featured_only: true
    design:
      view: article-grid
      columns: 2
      show_read_time: false       
  - block: collection
    content:
      title: All Publications
      text: ''
      filters:
        folders:
          - publications
        exclude_featured: false
    design:
      view: citation
      show_read_time: false   
  - block: collection
    id: confs
    content:
      title: Featured Confs
      filters:
        folders:
          - confs
    design:
      view: card
---
