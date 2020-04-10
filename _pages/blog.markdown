---
layout: archive
permalink: /blog/
title: Blog 
author_profile: false
sidebar:
  - image: "/assets/images/blog-cover.jpg"
description: "here's my blog. Full of crap but might be worth the read."
og_image: "/assets/images/blog-cover.jpg"
---
Here are sundry observations about events, travels, tech, art and other stuff about an ordinary life. If you like something or if you have a story of your own to share, please [write](mailto:letters@aravindiyer.com) to me.

## Latest Stories

<div class="grid__wrapper">
  {% assign posts = site.posts %}
  {% for post in posts %}
    {% include archive-single.html type="grid" %}
  {% endfor %}
</div>
