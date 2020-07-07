---
title: Guide for WordPress `Static sites`
date: 2020-07-07T09:59:09.988Z
menus:
  secondary:
    weight: 6
template: post
---
# WordPress Site

WordPress CMS brings together different multiple components - an Apache web server that serves up the code, an interpreted scripting language, PHP and a database server, MySQL. 

![](https://www.testandoptimize.com/images/68747470733a2f2f7265732e636c6f7564696e6172792e636f6d2f6d727961702f696d6167652f75706c6f61642f76313533393135373434382f776562736974652f7765626465762d737461636b2e6a7067.jpg)

Image Source: https://www.testandoptimize.com/posts/2018-09-29-From-LAMP-to-JAM/


When a content is posted on WordPress CMS, it will be saved in a mysql database (the database of WordPress). 

How do you backup the content on your WordPress? Remembered this content are store in database. It a chore to run phpmyadmin to access mysql to retrieve a content that up there.

![Mysql access via Adminer as I have wordpress content in sql.gz](https://pbs.twimg.com/media/DlISSUrWwAAbswE?format=jpg&name=900x900)

A workaround is via Github. All content is saved and store as markdown file. 

![](https://pbs.twimg.com/media/D5UNWEjWkAUPJXQ?format=jpg&name=900x900)

This Github as back-end approach is not for everyone as you need to master [Git command](https://mryap.github.io/github-oneliner/). 

### JamStack

Static websites are not a new concept. Before WordPress CMS, websites are crafted with html files, Css and javascript and being uploaded via FTP to a web server. No database is involved.

Smashing Magazine ditch WordPress and move to JAMstack - stands for JavaScript, APIs, & Markup; an approach to building and hosting websites that allows you to have all the web performance & security benefits of a static website along with the dynamic capabilities of a database-driven CMS.

static site are appealing for security, reliability, speed and saving on hosting site. Hosted on GitHub, powered by @Netlify with Content Delivery Network and free HTTPS. 

### The Best of Both World

Here my approach. You generate a WordPress site, de-couple from the CMS (which is a database) and served the published content. Without a round-trip request to the database to serve a webpage is appealing. A faster site and when your CMS is down, you site is still up and running.

### Caveat Emptor

You still can use WordPress CMS to insert new content as usual. However, you need to be aware of the following
- Any “real-time” dynamic content on your site will not woek
- WordPress built-in commenting system can't be use. If not even being use at all, you can do without it! 



