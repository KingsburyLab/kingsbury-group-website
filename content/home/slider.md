---
widget: slider
weight: 10
active: true
headless: true

design:
  # Slide height is automatic unless you force a specific height (e.g. '400px')
  slide_height: ''
  is_fullscreen: true
  # Automatically transition through slides?
  loop: true
  # Duration of transition between slides (in ms)
  interval: 7000

content:
  slides:
    - title: Welcome to the Kingsbury Research Group
      content: "We seek to **accelerate development** of electrochemical technologies that address environmental challenges related to climate change, water scarcity, and food security."
      align: center
      background:
        position: center
        color: '#666'
        brightness: 0.4
        media: Hero_1.jpg
        fit: cover
    - title: We study ion-selective materials
      content: 'Materials that filter charged particles (ions) are essential components of many clean water and energy technologies, including processes for **water desalination, wastewater recycling, energy storage,** and **energy production.**'
      align: left
      background:
        position: center
        color: '#555'
        brightness: 0.4
        media: Hero_2.jpg
        fit: cover
      link:
        icon: microscope
        icon_pack: fas
        text: Our Research
        url: ../research/
    - title: Join Us
      content: 'The Kingsbury Lab is coming to Princeton University! We are recruiting multiple graduate students and postdocs to start in Summer/Fall 2023.'
      align: left
      background:
        position: center
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
