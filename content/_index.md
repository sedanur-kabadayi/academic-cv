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
      headings:
        about: ''
        education: ''
        interests: ''
    design:
      spacing:
        padding: [0, 0, 0, 0]
      date_format: '2006-01'
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
  - block: resume-experience
    id: experience
    content:
      username: me
    design:
      date_format: 'Jan 2006'
      is_education_first: true
  - block: markdown
    content:
      title: '📚 My Research'
      subtitle: ''
      text: |-
        I work on finding allosteric and druggable pockets in viral polymerases.
        Before moving to computational work I spent several years in wet labs —
        peptide synthesis, extraction optimization, plant metabolomics.
        
        Feel free to reach out if any of this overlaps with what you do.
    design:
      columns: '1'
  - block: collection
    id: publications
    content:
      title: Publications
      filters:
        folders:
          - publications
        publication_type: 'article-journal'
    design:
      view: citation
  - block: collection
    id: conference
    content:
      title: Conference Papers
      filters:
        folders:
          - publications
        publication_type: 'paper-conference'
    design:
      view: citation
---
