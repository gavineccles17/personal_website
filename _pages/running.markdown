---
title: Running
permalink: "/running/"
layout: archive
author_profile: false
sidebar:
- image: "/assets/images/gavin9.jpg"
description: 'This page will document everything about running. '
og_image: "/assets/images/gavin8.jpg"
---

This page will document everything about running. [write](mailto:letters@aravindiyer.com) to me.

## Latest Stories

<div class="grid__wrapper">
  {% assign collection = 'running' %}
  {% assign posts = site[collection] | reverse %}
  {% for post in posts %}
    {% include archive-single.html type="grid" %}
  {% endfor %}
</div>
