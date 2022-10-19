---
layout              : default
show_meta           : false
title               : "Social Navigation"
subheadline         : "BIG Research"
teaser              : ""
header: no

widget1:
  title: "FRIDA: Robot Painting"
  url: '/research/frida'
  image: frida_timelapse.gif
  text: 'The FRIDA system supports real world image generation by taking inspiration from a human artist in multiple modalities and responds to noisy, stochastic execution with perception and replanning.'
widget2:
  title: "Near Real-Time Text-to-Video"
  url: 'https://pschaldenbrand.github.io/text2video/'
  text: 'Our system generates videos based on a series of language descriptions.'
  # video: '<a href="#" data-reveal-id="videoModal"><img src="http://phlow.github.io/feeling-responsive/images/start-video-feeling-responsive-302x182.jpg" width="302" height="182" alt=""/></a>'
  image: raven_small.gif
widget3:
  title: "Machine Traditional Animation: AniPainter"
  url: 'https://sites.gatech.edu/robotic-art-workshop/2021/07/02/anipainter/'
  image: coolin_painted.gif
  text: 'Using an affordable robot arm to "hand" paint animation frames.'

permalink           : "/research/social-navigation"
---

<div class="row">
    <h1>{{ page.title }}</h1>
    <p>At BIG, we are developing AI research that can support human creativity by empowering artists with barriers to engaging in the art world with tools to help them express themselves</p>
</div>

<div class="row t60">
    {% if page.widget1.image or page.widget1.video or page.widget1.title %}
        {% include _frontpage-widget.html widget=page.widget1 %}
    {% endif %}

    {% if page.widget2.image or page.widget2.video or page.widget2.title %}
        {% include _frontpage-widget.html widget=page.widget2 %}
    {% endif %}

    {% if page.widget3.image or page.widget3.video or page.widget3.title %}
        {% include _frontpage-widget.html widget=page.widget3 %}
    {% endif %}
</div><!-- /.row -->
