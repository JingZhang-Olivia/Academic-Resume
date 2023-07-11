---
# Leave the homepage title empty to use the site title
title:
date: 2023-6-22
type: landing

sections:
  - block: about.biography
    id: home
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin

  - block: collection
    id: publications
    content:
      title: Recent Publications
      text: |-
        {{% callout note %}}
        Quickly discover relevant content by [filtering publications](./publication/).
        {{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation


  - block: collection
    id: grants
    content:
      title: Selected Grants
      subtitle: ''
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        folders:
          - grants
    design:
      # Choose a layout view
#      view: compact
      columns: '2'


  - block: experience
    id: service
    content:
      title: Service and Awards
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: CEO
          company: GenCoin
          location: California
          date_start: '2021-01-01'
          date_end: ''

        - title: Professor of Semiconductor Physics
          company: University X
          location: California
          date_start: '2016-01-01'
          date_end: '2020-12-31'

        - title: Professor of Semiconductor Physics
          company: University X
          location: California
          date_start: '2016-01-01'
          date_end: '2020-12-31'
    design:
      columns: '2'


#  - block: collection
#    id: teaching
#    content:
#      title: Teaching Experience
#      filters:
#        folders:
#          - event
#    design:
#      columns: '2'
#      view: compact

  - block: collection
    id: teaching
    content:
      title: Teaching Experience
      subtitle: ''
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        folders:
          - post
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
      view: compact
      columns: '2'

  - block: collection
    id: team
    content:
      title: Team Members
      subtitle: ''
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        folders:
          - post
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
      view: compact
      columns: '2'


  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
       Feel free to contact me.
      # Contact (add or remove contact options as necessary)
      email: neilhengyun.li@polyu.edu.hk
      phone: +852 3400 2167
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      form:
        provider: netlify
        formspree:
          id:
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: false 
    design:
      columns: '2'
---
