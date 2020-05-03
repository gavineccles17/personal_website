---
title: How I created this website with Jekyll
date: '2020-04-25T16:30:38+01:00'
categories: Tech
tags: Tech
header:
  teaser: /assets/images/jekyll.png
excerpt: Website creation
description: A guide to creating your first static site
og_image: /assets/images/jekyll.png
---
{% include figure caption="Jekyll Website" image_path="jekyll.png" alt="Jekyll Website" %}

## Background Research

I set myself a target to create my own personal website. The purpose of the site was to create a space where I could write blog posts, document projects I am working on and as an attempt to learn web development.

My experience with web development is limited due a small project during college where we created a simple website with basic HTML, CSS, JS and PHP. This was mostly forgotten and meant I'd be starting from scratch so don't be put-off if this is your first time. 

I started researching on google how to make a website. Finding out that there are two types of websites that one can create: static or dynamic. Static sites are relatively simple, including pages with fixed content, like this static. Dynamic sites are more complicated, containing pages that change depending on the viewer, location, time of day etc. 

Static sites are perfect for sites where delivering information is the sole purpose. For example, a blogging platform or an online presence for small shops/companies. Dynamic sites are more suited if the site needs to take orders from customers and store customer information in databases. There seems to be a growing trend to move towards static sites due to their simplicity and fast loading times. 

Bearing that in mind, it was apparent that there are ample ways to make a website. Each varies in technical difficulty and in cost. Basically, the less programming you are willing to do, the higher the cost.

**Option 1:**

The first option is to use a web development service that uses drag and drop tools making it easy to create a website quickly and without much hassle. The two companies that were most prominent were Wix and Squarespace. You may be aware of them through their constant bombardment of ads on instagram. From a glance it seems that making a site quickly is relatively simple and the final products tend to look great. Bear in mind that it still takes time playing with the finicky stuff to perfect it. There are a range of price plans on offer depending on how complicated the website will be. The cost is around $90/year for the basic plan.  

**Option 2:**

The next option is to use Wordpress, a content management system (CMS) which is responsible for 35% of the websites you see today. Wordpress is capable of making fantastic websites but it seems like the learning curve is a bit higher. There are plenty of freelance Wordpress developers that do this as their full time job so it must require a bit more patience to create a site via Wordpress. From research, the popular option is to use wordpres.org and combine it with a hosting service like Bluehost to store your website. Wordpress is free but hosting your website (so it is visible online) is expensive with basic plans starting around $50/year. 

**Option 3:**

The other option is to code the website yourself requiring knowledge of some programming languages. This option may seem daunting but there are a number of tricks to get a basic site running quickly. For example, using static site generators like Jekyll or Pelican. A number of templates created by other developers are available to use as a starting point to build your website. Jekyll is free. The only cost entailed is if you want a custom domain name, it cost me $6/year. 

I would choose Option 1 or 2 if my website required facilitating customer purchasing or ordering. Note that you could also use Shopify to create a website and handle transactions for you. Furthermore, i would consider using Wordpress if you really wanted a website with that extra "wow factor". One should be aware that Wordpress sites require maintenance like updating packages/plugins. However, if simplicity, cost and no maintenance are priority then I would suggest considering Option 3 like I did. Read on and I'll show you how manageable it is.

Another option I recently came across was Google site builder which creates simple Websites, quickly and free too.

## Developing a static site

In order to go the more manual approach and create a static, you need to consider:

* Which site generator you will use. Most popular are Jekyll, Gatsby, Pelican, Hugo and Hexo.
* Where to host your site. Github pages is a free hosting service directly from your git repository. Netlify is another option which has a built in content delivery network.
* Optionally, pick a content management system (CMS) to easily facilitate blog creation using a UI tool rather than writing in markdown in code editors. Popular choices are: Siteleaf, Cloudcannon, forestry.io and Netlfiy. 

I went with Jekyll as it seemed to be the most popular and had a grand selection of templates I could use. I am a frequent user of Git for version control so Github pages was an obvious choice to store my site initially. Finally, I tried all of the aforementioned CMS platforms and ended up choosing Netlify. 

For this Blog, I will just include the articles and resources that helped me create a site rather than explain a step by step tutorial because that's just me re-writing someone else's work. In truth, this site took about 40 hours for me to do but a large part of this was due to researching, indecisiveness of theme and choosing images for my site. If I was to create a new site again, it would take a fraction of the time. Hopefully narrowing it down to the helpful resources below will minimise the time for you too.

There are two ways to create a jekyll website, either initialise one yourself or clone someone else's git project. This [article](http://www.stephaniehicks.com/githubPages_tutorial/pages/githubpages-jekyll.html) shows the simple steps for each one. I would recommend you do the first approach to quickly learn and get your head around how jekyll projects work and then do approach 2.

Follow this [article](https://www.taniarascia.com/make-a-static-website-with-jekyll/). You have to install a few dependencies...Ruby, Bundler, Jekyll and Git. Once all packages are installed, in two lines of code you have yourself a basic site available at a local host. Jump straight to the part where you push the site to your Github repository and you will have a site on Github pages for the world to see. 

Approach 2 enables you to skip all the initial design steps by using a template. There is a large amount of templates for Jekyll website and you should explore the following links until you find a template you think would suit your site. I would encourage you to spend time choosing as I made the mistake of changing my mind later on which wasted lots of time.

## **Jekyll Themes**

* List of the ones supported and maintained by Github. [Here](https://github.com/topics/jekyll-theme)
* 35 examples of cool themes. [Here](https://themefisher.com/best-jekyll-themes/)
* List of websites implementing the themes. [Here](https://github.com/jekyll/jekyll/wiki/sites)

There are a number of themes that you can purchase if none of the free ones suit your liking. These themes below were my favourite and took me awhile to choose between them. 

* [Mediumish](https://wowthemesnet.github.io/mediumish-theme-jekyll/)
* [Jasper2](https://jekyller.github.io/jasper2/)
* [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/)
* [Feeling Responsive](https://phlow.github.io/feeling-responsive/)

You can clone any of the sites on Github, maybe check for copyrights but most I saw were happy to allow you to clone.  

I initially went with Mediumish theme then switched to Feeling Responsive and finally settled on Minimal Mistakes. Mediumish looks like the blogging platform Medium, love the font. Feeling responsive is great, very well documented. Minimal Mistakes was my favourite as it is now supported by Github, works great on mobile, has detailed documentation and lots of room to edit and make it your own.

Following the documentation for minimal mistakes, all you have to do is edit the gem file on your current basic website and the theme will be install. A theme that is supported as a gemfile will hide some of the files like _includes, _sass, and /assets/. This is normal, all the files are stored in your Ruby library instead. (run this to see where 'bundle info minimal-mistakes-jekyll'
). Jekyll will use the files in your project first before falling back to the default versions of the theme. So you can overwrite and make changes if you wish. Just use the [documentation](https://mmistakes.github.io/minimal-mistakes/docs/quick-start-guide/#ruby-gem-method) for creating new pages and posts and it will be self explanatory. 

If you get confused, you are welcome to clone [my repository](https://github.com/gavineccles17/personal_website) and use this as your starting point.

I used [this site](https://www.aravindiyer.com/) as a guideline for making my site. He has a number of helpful tutorials for using Minimal mistakes theme. 

In the minimal mistakes documentation, you will find steps to do the following and more:

* Site verification with Bing and Google.
* Setting up Google Analytics
* Creating site logo and favicons
* Enabling comments on articles
* Adding site searches

## Setting up a Domain Name System (DNS)

Github gives you a site like "http(s)://<username>.github.io/<projectname>" but if you want to have a custom domain you will have to implement a few extra steps and incur a small fee. It's worth it though! It doesn't take long, just need to add a file to your github called CName then point your DNS provider to your Github repo. It went with register365 for my DNS provider, in hindsight I would have went with Google as there's my documentation online if things get confusing. Also be aware that it takes a few hours for your site to be live.

* [Easy tutorial](https://medium.com/@xiang_zhou/how-to-add-custom-domain-to-your-jekyll-blog-provided-that-you-built-your-site-using-github-6e1c8bf20afe)
* [Troubleshooting](https://stackoverflow.com/questions/9082499/custom-domain-for-github-project-pages)

## **Comparing different CMS tools**

After spending a number of hours creating and designing the website, I wanted to use a CMS platform so I could easily make blogs and upload pictures in the future. This removes the hassle of doing git versions and changes in a code editor. Instead, you get a handy UI tool where you can edit content which pushes straight to Github for you. These are the CMS's I investigated. The basic plans on all of these are free and this is all you should need.

* **Forestry.io.** It looks very professional for a client especially if the purpose is just to make blogs. However, a lack of documentation and what seemed simple like importing files was not. Also the preview was quite slow.
* **Siteleaf.com.** It doesn't look great, quite childish. Better for developer as you can see all the files but you can’t click into it. Couldn’t seem to get certain pages showing.
* **Cloudcannon.** I thought cloudcannon was good for my initial site theme as it has a live dashboard and can view/edit straight from URL. However, it was not compatible with the jekyll version for my final site which was a pity.
* **Netlify.** This was the last one I tried and it was brilliant. I was apprehensive at first because you have to switch your host from Github to Netlify. It still uses git for version control just not hosting. This was not too difficult, it just involved redirecting to Netlfiy from DNS provider, [tutorial here](https://medium.com/@yashjoshi76/host-your-github-page-on-a-custom-domain-using-netlify-287850650d75). Netlfiy has CI/CD (continuous integration/continuous deployment) which enables you to make changes review them later and confirm to push. The best part is you can make changes directly on your website in your browser (like I am now, see below).

![Currently writing this blog in browser](/assets/images/screenshot-2020-04-25-at-21.41.51.png)

And there you have it, how i managed to create this site. Next, I plan on looking at creating a site with Wordpress then comparing them. 

I hope this article will simplify the task for yourself and help you make amazing websites!

Slán go fóill,

Gavin
