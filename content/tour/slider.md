---
widget: slider
weight: 1
active: true
headless: true

design:
  # Slide height is automatic unless you force a specific height (e.g. '400px')
  slide_height: ''
  is_fullscreen: true
  # Automatically transition through slides?
  loop: false
  # Duration of transition between slides (in ms)
  interval: 2000

content:
  slides:
    - title: Welcome to the Kingsbury Research Group
      content: ![kingsbury lab logo](kingsbury_lab_logo.png)We seek to **accelerate development** of electrochemical technologies that address environmental challenges related to climate change, water scarcity, and food security.
      align: center
      background:
        position: right
        color: '#666'
        brightness: 0.5
        media: Hero_1.jpg
        fit: cover
    - title: We study ion-selective materials
      content: 'Materials that filter charged particles (ions) are essential components of new clean technologies for water purification and energy production.'
      align: left
      background:
        position: center
        color: '#555'
        brightness: 0.5
        media: Hero_2.jpg
        fit: cover
      link:
        icon: microscope
        icon_pack: fas
        text: Our Research
        url: ../research/
    - title: Join Us
      content: 'The Kingsbury Group is coming to Princeton University! We are recruiting multiple graduate students and postdocs to start in Summer/Fall 2023.'
      align: right
      background:
        position: right
        color: '#333'
        brightness: 0.5
        media: Hero_5.jpg
        fit: cover
      link:
        icon: graduation-cap
        icon_pack: fas
        text: See Openings
        url: ../people/
---
