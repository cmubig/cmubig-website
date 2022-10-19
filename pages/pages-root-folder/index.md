---
#
# Use the widgets beneath and the content will be
# inserted automagically in the webpage. To make
# this work, you have to use › layout: frontpage
#
layout: frontpage
header:
  image_fullwidth: big-summer2018.jpg
widget1:
  title: "FRIDA: Robot Painting"
  url: '/research/frida'
  image: frida_timelapse.gif
  text: 'The FRIDA system supports real world image generation by taking inspiration from a human artist in multiple modalities and responds to noisy, stochastic execution with perception and replanning.'
widget2:
  title: "How do you train AI Pilots?"
  url: 'http://phlow.github.io/feeling-responsive/info/'
  text: 'description'
  image: ai_pilot.jpeg
widget3:
  title: "Near Real-Time Text-to-Video"
  url: 'https://pschaldenbrand.github.io/text2video/'
  text: 'Our system generates videos based on a series of language descriptions.'
  # video: '<a href="#" data-reveal-id="videoModal"><img src="http://phlow.github.io/feeling-responsive/images/start-video-feeling-responsive-302x182.jpg" width="302" height="182" alt=""/></a>'
  image: raven_small.gif
#
# Use the call for action to show a button on the frontpage
#
# To make internal links, just use a permalink like this
# url: /getting-started/
#
# To style the button in different colors, use no value
# to use the main color or success, alert or secondary.
# To change colors see sass/_01_settings_colors.scss
#
callforaction:
  url: https://tinyletter.com/feeling-responsive
  text: Inform me about new updates and features ›
  style: alert
permalink: /index.html
#
# This is a nasty hack to make the navigation highlight
# this page as active in the topbar navigation
#
homepage: true
---

<div id="videoModal" class="reveal-modal large" data-reveal="">
  <div class="flex-video widescreen vimeo" style="display: block;">
    <iframe width="1280" height="720" src="https://www.youtube.com/embed/3b5zCFSmVvU" frameborder="0" allowfullscreen></iframe>
  </div>
  <a class="close-reveal-modal">&#215;</a>
</div>
