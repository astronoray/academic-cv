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
      text: 'Hello! My name is Ray Garner, and I am a postdoc in the [Astronomy Group at Texas A&M University](https://physics.tamu.edu) in College Station, Texas. I am an observational astronomer interested in how we use nebular emission lines to understand the physical conditions and evolution of galaxies. These lines let us measure properties such as chemical abundances, ionization, gas temperatures and densities, dust extinction, and kinematics, but interpreting them requires assumptions about the stars, gas, geometry, and environments that produce them. Much of my research asks how well those assumptions hold. <br><br> My work spans the nearby Universe to Cosmic Dawn. As a member of the Star formation, Ionized Gas, and Nebular Abundances Legacy Survey ([SIGNALS](https://signal-survey.org/)) collaboration, I use spatially resolved spectroscopy of nearby H&nbsp;<span style="font-size: 0.8em;">II</span> regions to study nebular diagnostics, stellar feedback, chemical abundances, and ionized-gas kinematics. I also maintain a long-running research program on the nearby M101 Group, using imaging and integral-field spectroscopy to connect star formation, stellar populations, chemical evolution, spiral structure, and galaxy interactions. More recently, I have extended this work to galaxies in the Epoch of Reionization using JWST/NIRSpec rest-frame UV and optical spectroscopy to investigate extreme nebular conditions and the sources of highly energetic ionizing radiation. <br><br> Before coming to Texas A&M, I earned my Ph.D. in Astronomy from [Case Western Reserve University](https://astronomy.case.edu/), where I worked with [Prof. Chris Mihos](https://burro.case.edu/) on the evolution of M101 and its satellite group using deep, wide-field imaging from the Burrell Schmidt telescope. I received my B.S. in Physics, *summa cum laude*, from [Furman University](https://www.furman.edu), where I first became involved in astronomical research.' 
    

      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/resume_cv.pdf
      headings:
        about: ''
        education: ''
        interests: ''
    design:
      # Use the new Gradient Mesh which automatically adapts to the selected theme colors
      background:
        gradient_mesh:
          enable: false

      # Name heading sizing to accommodate long or short names
      name:
        size: md # Options: xs, sm, md, lg (default), xl

      # Avatar customization
      avatar:
        size: large # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded
  # - block: markdown
  #   content:
  #     title: '📚 My Research'
  #     subtitle: ''
  #     text: |-
  #       Use this area to speak to your mission. I'm a research scientist in the Moonshot team at DeepMind. I blog about machine learning, deep learning, and moonshots.

  #       I apply a range of qualitative and quantitative methods to comprehensively investigate the role of science and technology in the economy.

  #       Please reach out to collaborate 😃
  #   design:
  #     columns: '1'
  - block: collection
    id: papers
    content:
      title: Recent Publications
      filters:
        folders:
          - publications
        featured_only: true
    design:
      view: article-grid
      columns: 1
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
  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      count: 4
      filters:
        folders:
          - events
    design:
      view: article-grid
  - block: collection
    id: news
    content:
      title: Recent Posts
      subtitle: ''
      text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: blog
      # Choose how many pages you would like to display (0 = all pages)
      count: 4
      # Filter on criteria
      filters:
        author: ''
        category: ''
        tag: ''
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ''
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: article-grid
      # Reduce spacing
      spacing:
        padding: [0, 0, 0, 0]
  - block: contact-info
    content:
      title: Contact Me! 
      subtitle: 
      connect_title: Send me a message!
      text: I'm always open to chatting with folks about science!
      # visit_title: 
      # connect_title: 
      # address:
      #   lines:
      #     - 4242 TAMU
      #     - College Station, TX 77843
      #     - United States
      office_hours:
      email: ray.garner at tamu.edu
      phone: 
      social:
        - icon: brands/instagram
          url: https://www.instagram.com/astronoray
        - icon: brands/linkedin
          url: https://www.linkedin.com/in/ray-garner-bb3143b8/
        - icon: brands/bluesky
          url: https://bsky.app/profile/astronoray.bsky.social
        - icon: brands/youtube
          url: https://www.youtube.com/channel/UCJmyKp5pHuy_yCg5IJGkvQQ
        - icon: brands/github
          url: https://github.com/astronoray
      # prospective:
      #   title: Prospective Members
      #   text: Interested in joining our lab? We're looking for motivated researchers.
      #   button:
      #     text: View Open Positions
      #     url: /opportunities
      map_url: 
      show_form: false
    # design:
    #   css_class: "bg-gray-50 dark:bg-gray-900"
    #   spacing:
    #     padding: ["3rem", 0, "3rem", 0]
  # - block: contact-info
  #   content:
  #     title: Contact
  #     email: ray.garner at tamu.edu
  #     address:
  #       street: 4242 TAMU
  #       city: College Station
  #       region: TX
  #       postcode: '77843'
  #       country: United States
  #       country_code: US
  # - block: cta-card
  #   demo: true # Only display this section in the HugoBlox Kit demo site
  #   content:
  #     title: 👉 Build your own academic website like this
  #     text: |-
  #       This site is generated by HugoBlox Kit - the FREE, Hugo-based open source website builder trusted by 250,000+ academics like you.

  #       <a class="github-button" href="https://github.com/HugoBlox/kit" data-color-scheme="no-preference: light; light: light; dark: dark;" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star HugoBlox/kit on GitHub">Star</a>

  #       Easily build anything with blocks - no-code required!

  #       From landing pages, second brains, and courses to academic resumés, conferences, and tech blogs.
  #     button:
  #       text: Get Started
  #       url: https://hugoblox.com/templates/
  #   design:
  #     card:
  #       # Card background color (CSS class)
  #       css_class: 'bg-gradient-to-br from-primary-500 via-primary-600 to-secondary-600 text-white shadow-2xl'
  #       css_style: ''
---
