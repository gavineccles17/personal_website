---
layout: archive 
permalink: /photography/
title: Photography
author_profile: false
sidebar:
  - image: "/assets/images/photography-cover.jpg"
description: "This page will show all my photographs as I strive to become a good photographer."
toc: true
og_image: "/assets/images/land2.jpg"
---
This page will show all my photographs as I strive to become a good photographer.

## Latest stories

<div class="grid__wrapper">
  {% assign collection = 'photography' %}
  {% assign posts = site[collection] | reverse %}
  {% for post in posts %}
    {% include archive-single.html type="grid" %}
  {% endfor %}
</div>
