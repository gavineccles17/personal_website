---
layout: archive 
permalink: /photography/
title: Music Naka
author_profile: false
sidebar:
  - image: "/assets/images/photography-cover.jpg"
description: "Music makes its best impression when it is shared by a friend over a story. Music is a medium for communicating and stimulating emotions, for conveying the mood, feelings, state of mind and even the sense of identity of the artist, and of the audience too. The stories on this page aim to help you know more about this context behind the music, so that you can connect more deeply with it. It's good seeing you at Music Naka! If you like a story or if you have one to share, please write to me."
toc: true
og_image: "/assets/images/photography-cover.jpg"
---
Music makes its best impression when it is shared by a friend over a story. Music is a medium for communicating and stimulating emotions, for conveying the mood, feelings, state of mind and even the sense of identity of the artist, and of the audience too. The stories on this page aim to help you know more about this context behind the music, so that you can connect more deeply with it. It's good seeing you at Music Naka! If you like a story or if you have one to share, please [write](mailto:letters@aravindiyer.com) to me. If it interests you, [read more]({{ site.baseurl }}{% link _pages/photography-background.markdown %}) about the story behind Music Naka.

## Latest stories

<div class="grid__wrapper">
  {% assign collection = 'photography' %}
  {% assign posts = site[collection] | reverse %}
  {% for post in posts %}
    {% include archive-single.html type="grid" %}
  {% endfor %}
</div>
