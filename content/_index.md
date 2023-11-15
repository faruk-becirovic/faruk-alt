---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: features
    content:
      title: Skills
      items:
        - name: Python
          description:
          icon: python
          icon_pack: fab
        - name: R
          description: 
          icon: r-project
          icon_pack: fab
        - name: Statistics
          description:
          icon: chart-simple
          icon_pack: fas
        - name: Bioinformatics
          icon: dna
          icon-pack: fas
        - name: Data Engineering
          icon: database
          icon-pack: fas
        - name: Data Analysis
          icon: chart-pie
          icon-pack: fas
  - block: experience
    content:
      title: Experience
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: System Engineer
          company: Verlab Institute
          company_url: 'https://verlabinstitute.com/'
          company_logo: 
          location: Sarajevo, BiH
          date_start: '2023-07-01'
          date_end: ''
          description: Participated on various research projects conducted at the institute in the field of bioinformatics and artificial intelligence. Worked on development of ML models, as well as development of REST API using Django, deploying the API and managing the development environment. Furthermore, I have worked on preparing research papers for publication.
        - title: Software Developer
          company: Digiqal
          company_url: 'https://digiqal.de/'
          company_logo: 
          location: Munich, DE (Remote)
          date_start: '2022-07-01'
          date_end: '2022-10-01'
          description: Full-stack software developer with focus on front-end development.
        - title: Data Analyst
          company: SOCIALEXPLORER
          company_url: 'https://www.socialexplorer.com/'
          company_logo: 
          location: Sarajevo, BiH
          date_start: '2021-11-01'
          date_end: '2022-03-31'
          description: Collection of data using web-scraping techniques, import, inspection, cleaning, transformation and validation of data.
    design:
      columns: '2'
  - block: collection
    id: posts
    content:
      title: Recent Posts
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
  - block: portfolio
    id: projects
    content:
      title: Projects
      filters:
        folders:
          - project
      # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
      default_button_index: 0
      # Filter toolbar (optional).
      # Add or remove as many filters (`filter_button` instances) as you like.
      # To show all items, set `tag` to "*".
      # To filter by a specific tag, set `tag` to an existing tag name.
      # To remove the toolbar, delete the entire `filter_button` block.
      buttons:
        - name: All
          tag: '*'
        - name: Deep Learning
          tag: Deep Learning
        - name: Other
          tag: Demo
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
  - block: markdown
    content:
      title: Gallery
      subtitle: ''
      text: |-
        {{< gallery album="demo" >}}
    design:
      columns: '1'
  - block: collection
    id: featured
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: card
  - block: collection
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
    id: events
    content:
      title: Recent & Upcomin Events
      filters:
        folders:
          - event
    design:
      columns: '2'
      view: compact
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle: Talk to me
      text: |-
        If you have an interesting project or collaboration proposal, or if you would just like to chat, feel free to send me a message or make an appointment.
      # Contact (add or remove contact options as necessary)
      appointment_url: 'https://calendly.com/farukbecc'
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
