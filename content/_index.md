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
#        exclude_featured: true
    design:
      columns: '2'
      view: citation

  - block: collection
    id: grants
    content:
      title: Selected Grants
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation

  - block: experience
    id: service
    content:
      title: service and awards
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

  - block: accomplishments
    id: teaching
    content:
#      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      title: Teaching Experience
      subtitle:
      # Date format: https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
#      Accomplishments.
      #   Add/remove as many `item` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
#        - certificate_url: https://www.coursera.org
          date_end: ''
          date_start: '2021-01-25'
          description: ''
          organization: Coursera
#          organization_url: https://www.coursera.org
          title: Neural Networks and Deep Learning
#          url: ''
#        - certificate_url: https://www.edx.org
          date_end: ''
          date_start: '2021-01-01'
          description: Formulated informed blockchain models, hypotheses, and use cases.
          organization: edX
#          organization_url: https://www.edx.org
          title: Blockchain Fundamentals
#          url: ''

#        - certificate_url: https://www.datacamp.com
          date_end: '2020-12-21'
          date_start: '2020-07-01'
          description: ''
          organization: DataCamp
#          organization_url: https://www.datacamp.com
          title: 'Object-Oriented Programming in R'
#          url: ''
#    design:
#      columns: '2' 

  - block: collection
    id: team
    content:
      title: Qualifications
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
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam mi diam, venenatis ut magna et, vehicula efficitur enim.
      # Contact (add or remove contact options as necessary)
      email: neilhengyun.li@polyu.edu.hk
      phone: +852 3400 2167
      # Automatically link email and phone or display as text?    
    design:
      columns: '2'
---
