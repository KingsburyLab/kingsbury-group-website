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
    - title: 👋 Welcome to the group
      content: Take a look at what we're working on...
      align: center
      background:
        position: right
        color: '#666'
        brightness: 0.7
        media: Hero_1.jpg
        fit: contain
    - title: Lunch & Learn ☕️
      content: 'Share your knowledge with the group and explore exciting new topics together!'
      align: left
      background:
        position: center
        color: '#555'
        brightness: 0.7
        media: Hero_2.jpg
        fit: contain
    - title: Join Us
      content: 'The Kingsbury Group is coming to Princeton University in 2023!'
      align: right
      background:
        position: center
        color: '#333'
        brightness: 0.5
        media: Hero_5.jpg
        fit: contain
      link:
        icon: graduation-cap
        icon_pack: fas
        text: Opportunities
        url: ../people/
---
