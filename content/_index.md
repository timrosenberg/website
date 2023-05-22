---
# Leave the homepage title empty to use the site title
title: 'Timothy Rosenberg: Saxophonist, Teacher, Technologist'
date: 2023-05-17
type: landing

#######################
#      HERO BLOCK     #
#######################

sections:
- block: hero
  content:
    title: Hello!
    image: 
      filename: circle-headshot.png
    text: |-
      **I'm a saxophonist and music educator who has been teaching at colleges and universities for over eleven years.**

      **I specialize in classical, avant-garde, jazz, and commercial music.**

      Currently, I teach saxophone at Stetson University. I have also taught at Bethune-Cookman University, Full Sail Univeristy, and Ithaca College.
  design:
    background:
      gradient_end: '#429C80'
      gradient_start: '#006747'
      text_color_light: true
      image:
        filename: background-image.png
        size: cover
        position: center
        parallax: false
      
#######################
#      BIO BLOCK      #
#######################

- block: about.biography
  id: about
  content:
    title: Biography
    # Choose a user profile to display (a folder name within `content/authors/`)
    username: admin
# - block: features
#     content:
#       title: Skills
#       items:
#         - name: R
#           description: 90%
#           icon: r-project
#           icon_pack: fab
#         - name: Statistics
#           description: 100%
#           icon: chart-line
#           icon_pack: fas
#         - name: Photography
#           description: 10%
#           icon: camera-retro
#           icon_pack: fas

#######################
#  EXPERIENCE BLOCK   #
#######################

- block: experience
  id: experience
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
      - title: Visiting Assistant Professor of Saxophone
        company: Stetson University
        company_url: 'http://www.stetson.edu'
        company_logo: stetson-seal
        location: DeLand, FL
        date_start: '2022-08-15'
        date_end: ''
        description: |2-
            Responsibilities include:

            * Saxophone
            * Chamber Music
            * Improvisation
      - title: Adjunct Instructor of Saxophone
        company: Bethune-Cookman University
        company_url: 'http://www.cookman.edu'
        company_logo: bcu-seal
        location: Daytona Beach, FL
        date_start: '2016-08-15'
        date_end: '2022-05-15'
        description: Taught saxophone lessons and chamber music.
      - title: Course Director of Music Business
        company: Full Sail University
        company_url: 'http://www.fullsail.edu'
        company_logo: full-sail-seal
        location: Winter Park, FL
        date_start: '2012-03-05'
        date_end: '2023-08-11'
        description: Teach _Talent Evaluation for A&R_ and other courses in Music Business.
      - title: Assistant Professor of Saxophone (Sabbatic Replacement)
        company: Ithaca College
        company_url: 'http://ithaca.edu'
        company_logo: ithaca-seal
        location: Ithaca, NY
        date_start: '2010-08-15'
        date_end: '2011-08-15'
        description: Taught saxophone lessons and chamber music.    
  design:
    columns: '2'
- block: portfolio

#######################
#  PERFORMANCES BLOCK #
#######################

  id: performances
  content:
    title: Performances
    filters:
      folders:
        - project
  design:
    columns: '1'
    view: showcase
    flip_alt_rows: false
- block: accomplishments

#########################
# ACCOMPLISHMENTS BLOCK #
#########################

  id: accomplishments
  content:
    # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
    title: 'Accomplish&shy;ments'
    subtitle:
    # Date format: https://wowchemy.com/docs/customization/#date-format
    date_format: Jan 2006
    # Accomplishments.
    #   Add/remove as many `item` blocks below as you like.
    #   `title`, `organization`, and `date_start` are the required parameters.
    #   Leave other parameters empty if not required.
    #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
    items:
      - certificate_url: 
        date_end: ''
        date_start: '2016-07-07'
        description: ''
        organization: Full Sail University
        organization_url: http://www.fullsail.edu
        title: PROPS Top 10% Award for Excellence in Teaching
        url: ''
      - certificate_url: 
        date_end: ''
        date_start: '2015-07-06'
        description: ''
        organization: Full Sail University
        organization_url: http://www.fullsail.edu
        title: PROPS Certificate of Recognition for Excellence in Teaching
        url: ''
      - certificate_url: 
        date_end: ''
        date_start: '2009-02-15'
        description: ''
        organization: Michigan State University
        organization_url: https://www.msu.edu
        title: 'Michigan State University Honors Competition: Finalist'
        url: ''
  design:
    columns: '2'

#######################
#   BLOG POSTS BLOCK  #
#######################

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


#######################
#    PHOTOS BLOCK     #
#######################
- block: markdown
  id: gallery
  content: 
    title: Gallery
    text: |
      {{< gallery album="homepage" >}}

#######################
#  CONFERENCES BLOCK #
#######################
- block: collection
  id: conferences
  content:
    title: Recent Con&shy;ference Presen&shy;tations
    count: 3
    filters:
      folders:
        - event
      tag: "Conferences"
    archive:
      enable: true
      text: See All Conferences
  design:
    columns: '2'
    view: compact

#######################
#    EVENTS BLOCK     #
#######################

- block: collection
  id: events
  content:
    title: Recent & Upcoming Events
    count: 3
    filters:
      folders:
        - event
      tag: "Performances"
    archive:
      enable: true
      text: See All Events
  design:
    columns: '2'
    view: compact

#######################
#    CONTACT BLOCK    #
#######################

- block: contact
  id: contact
  content:
    title: Contact
    subtitle:
    text: |-
      Send me your questions, thoughts, dream diarys, hopes, _fears_, recipes, secrets, short stories, poems, and really good jokes. 
    # Contact (add or remove contact options as necessary)
    # email: test@example.org
    # phone: 888 888 88 88
    # appointment_url: 'https://calendly.com'
    address:
      street: 421 Woodland Blvd.
      city: DeLand
      region: FL
      postcode: '32723'
      country: United States
      country_code: US
    # directions: Enter Building 1 and take the stairs to Office 200 on Floor 2
    # office_hours:
    #   - 'Monday 10:00 to 13:00'
    #   - 'Wednesday 09:00 to 10:00'
    contact_links:
      - icon: mastodon
        icon_pack: fab
        name: DM Me
        link: 'https://mastodon.social/timrosenberg'
      - icon: facebook
        icon_pack: fab
        name: Friend Me
        link: 'http://www.facebook.com/timothyrosenberg'
      - icon: youtube
        icon_pack: fab
        name: Watch Me
        link: 'http://www.youtube.com/timothyrosenberg'  
      - icon: instagram
        icon_pack: fab
        name: Look at My Pics 🤷‍♂️
        link: 'https://instagram.com/timothyrosenberg'
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

#######################
#  GALLERY CAPTIONS   #
#######################

gallery_item:
- album: homepage
  image: 2023-Feb-21-Poster.png
  caption: "Recital Poster for my Faculty Recital in 2023 featuring music by composers from under-represented groups for tenor saxophone. The complete recital can be streamed [here](/event/faculty-recital-music-for-tenor-saxophone-by-diverse-composers/)"

- album: homepage
  image: hippocrene-quartet-2023.jpg
  caption: "This is the caption."

- album: homepage
  image: sax-camp-2022-large-ensemble.jpg
  caption: "This is the caption."

- album: homepage
  image: sax-camp-2022-large-ensemble.jpg
  caption: "This is the caption."

- album: homepage
  image: Stetson_SOM_1510.jpg
  caption: "This is the caption."

- album: homepage
  image: Stetson_SOM_1546.jpg
  caption: "This is the caption."

- album: homepage
  image: vertical-with-soprano.jpg
  caption: "This is the caption."
---
