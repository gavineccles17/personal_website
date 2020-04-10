---
layout: archive
permalink: /blog/
title: Blog 
author_profile: false
sidebar:
  - image: "/assets/images/blog-cover.jpg"
description: "This is where all my blogs will be archived. Full of crap but might be worth the read."
og_image: "/assets/images/blog-cover.jpg"
---
This is where all my blogs will be archived. Full of crap but might be worth the read. [write](mailto:letters@aravindiyer.com) to me.

## Latest Stories

<div class="grid__wrapper">
  {% assign posts = site.posts %}
  {% for post in posts %}
    {% include archive-single.html type="grid" %}
  {% endfor %}
</div>
