---
title: Guide for WordPress `Static sites`
subtitle: Made WordPress Load Faster in half-a-day without static site generators
date: 2020-07-07T09:59:09.988Z
thumb_img_path: /images/wp-super-cache-advanced-tab-settings-crunchify-tips.png
menus:
  secondary:
    weight: 6
template: post
---
WordPress Site works with PHP and MySQL. WordPress brings together multiple components - an Apache web server that serves up the code, an interpreted scripting language, PHP and a database server, MySQL. 

When a page loads on the browser, the core PHP files will pull data and instructions from the database to assemble the page. It happens dynamically each time.  

![](https://www.testandoptimize.com/images/68747470733a2f2f7265732e636c6f7564696e6172792e636f6d2f6d727961702f696d6167652f75706c6f61642f76313533393135373434382f776562736974652f7765626465762d737461636b2e6a7067.jpg)

Image Source: https://www.testandoptimize.com/posts/2018-09-29-From-LAMP-to-JAM/

When a content is posted on WordPress CMS, it will be saved in a MySQL database (the database of WordPress). 

How do you backup the content on your WordPress? Remembered this content are store in database. It a really hassle to run phpmyadmin to access mysql to retrieve a content that being uploaded.

![Mysql access via Adminer so I can have wordpress content in sql.gz](https://pbs.twimg.com/media/DlISSUrWwAAbswE?format=jpg&name=900x900)

### JamStack

Static websites are not a new concept. Before WordPress CMS, websites are built with html files, CSS and Javascript and being uploaded via FTP to a web server. No database is involved.

JAMstack - stands for JavaScript, APIs, & Markup; is an approach to building and hosting websites that allows you to have all the web performance & security benefits of a static website along with the dynamic capabilities of a database-driven CMS. Smashing Magazine ditch WordPress and move to JAMstack. 

As database is not involve each time, static sites are appealing for their security, reliability, speed and saving on hosting site. 

### The Best of Both World

Without a round-trip request to the database to served up a webpage when user access thru a browser is appealing. A faster site and when your CMS is down, you site will not be affected

A workaround via Github. All content is saved and store as markdown file. 

![Image of  a GitHub folder where websites files are stored and served. ](/images/screenshot_2020-09-28-d5unwejwkaupjxq-jpeg-image-900-×-473-pixels-.png)

This Github as back-end approach is not for everyone as you need to master [Git command](https://mryap.github.io/github-oneliner/).

### Made WordPress Load Faster without static site generators

Another approach is to use `WP Super Cache plugin`. The plugin generates static html files from your dynamic WordPress blog. After a html file is generated and available under/cache folder, your Web Server will serve that static file instead of processing the comparatively heavier and more expensive WordPress PHP scripts

![Speed up WordPress Site by tuning WP Super Cache Settings](/images/wp-super-cache-advanced-tab-settings-crunchify-tips.png)

### Caveat Emptor - The Trade Off

You need to be aware of the following if you decide to go 'static`

* Any “real-time” dynamic content on your site will not work
* WordPress built-in commenting system can't be use. (If not even being use at all, you can do without it!) 

If you already have an existing WordPress site that doing well for your organization, here is a case study that helps to speed up WordPress site without going 'static' [link](https://www.wpbeginner.com/opinion/how-we-made-wordpress-faster-than-static-site-generators-case-study-speeding-up-wpbeginner/?utm_source=testandoptimize.com)

#### End Note: How fast is fast?

There isn't a universal definition of “fast” vs “slow.” Speed, i.e the loading time of your site is the most important metric 
My assertion: Take action if your site page loading speed > 15 seconds [Time to Interactive (TTI)](https://web.dev/interactive/)!

#### Hire Me

I migrated an Irish SMB's WordPress site to a new hosting provider without losing any content. On another project, I use WP Fastest Cache, image scaling and WP Smush to improve the WordPress website performance. I can help to improve your WordPress site, add features, improve usability and search rankings.