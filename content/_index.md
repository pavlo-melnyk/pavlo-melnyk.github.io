---
# Leave the homepage title empty to use the site title
title: ""
date: 2024-10-20
type: landing

design:
  # Default section spacing
  spacing: "5rem"

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
      # button:
      #   text: CV
      #   url: uploads/resume.pdf
      # button:
      #   text: PhD thesis
      #   url: https://doi.org/10.3384/9789180756808
    design:
      css_class: dark
      background:
        color: black
        image:
          # Add your image background to `assets/media/`.
          filename: flower_of_life.png # stacked-peaks.svg
          filters:
            brightness: .5
          size: cover
          position: center
          parallax: false
  - block: collection
    id: papers
    content:
      title: 'Featured Publications'
      filters:
        folders:
          - publication
        featured_only: true
    design:
      view: article-grid
      columns: 2
  - block: collection
    content:
      title: 'Publications'
      text: 
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: citation
  - block: collection
    id: news
    content:
      title: News
      subtitle: ''
      text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: post
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: date-title-summary
      # Reduce spacing
      spacing:
        padding: [1, 1, 1, 1]
  # - block: markdown
  #   content:
  #     title: ''
  #     subtitle: ''
  #     text: |-
  #           You can view all my publications on [<u>Google Scholar</u>](https://scholar.google.com/citations?user=RhThiI8AAAAJ&hl=en) {{< icon name=\"academicons/google-scholar\" >}}.
  #   design:
  #     columns: '1'
  # - block: collection
  #   id: talks
  #   content:
  #     title: Recent & Upcoming Talks
  #     filters:
  #       folders:
  #         - event
  #   design:
  #     view: article-grid
  #     columns: 1
---
