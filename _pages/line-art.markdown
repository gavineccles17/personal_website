---
title: Line Art
permalink: "/line-art/"
layout: archive
author_profile: false
description: I am Aravind, a tech guy, a scientist and computer engineer by training,
  dabbling with line art. My posts on line art present my drawings, techniques and
  motivations behind the work.
og_image: "/assets/images/self-sketch-splash.jpg"
---

<div class="grid__wrapper">
  {% assign category = 'line-art' %}
  {% assign posts = site.categories[category] %}
  {% for post in posts %}
    {% include archive-single.html type="grid" %}
  {% endfor %}
</div>
