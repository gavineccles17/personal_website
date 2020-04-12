---
title: Blog
permalink: "/blog/"
layout: archive
author_profile: true
header:
  image: /assets/images/costa_rica.jpg
  caption: Costa Rica
description: This is where my latest blogs will appear
---

This is where my latest blogs will appear. Some of the topics I have planned for my blogs:

* Technology
* Travel
* Running
* Photography
* Books
* Motivation
* Life in General 

The first blogs that I have to write on my list are:
1.	How I setup a website 
1.	Dealing with the Corona Virus

Please [reach out to me]({{ site.baseurl }}/contact/) if anyone has any topics they feel would be good to discuss, thanks!

## Latest Stories

<div class="grid__wrapper">
  {% assign posts = site.posts %}
  {% for post in posts %}
    {% include archive-single.html type="grid" %}
  {% endfor %}
</div>
