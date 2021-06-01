---
title: Mindful of Your Parameter URLs
date: 2021-06-01T10:26:33.109Z
template: post
---
The most common use cases for parameters are:

* **Tracking** –  ?utm_medium=social, ?sessionid=123 or ?affiliateid=abc
* **Reordering** –  ?sort=lowest-price, ?order=highest-rated or ?so=newest
* **Filtering** –  ?type=widget, colour=blue or ?price-range=20-50
* **Identifying** – ?product=small-blue-widget, categoryid=124 or itemid=24AU
* **Paginating** – ?page=2, ?p=2 or viewItems=10-30
* **Searching** –  ?query=users-query, ?q=users-query or ?search=drop-down-option
* **Translating** – ?lang=fr, ?language=de or

### Problem with URL Parameters
Parameter URLs are all well and good until they’re hit by a ton of traffic and become a nuisance. This inundation of traffic can result in reports hundreds of pages long.  

If you know that certain parameter URLs should not be tracked, filter them out of your Google Analytics reports.  

By filtering out parameter URLs where they make sense, you improve the accuracy of your tracking and create better attribution models for your search traffic.

[How To Exclude URL Query Parameters in Google Analytics](https://www.bounteous.com/insights/2020/05/15/excluding-url-query-parameters-google-analytics/)



<!--StartFragment-->

**Look in Google Analytics All Pages report**: Search for “?” to see how each of the parameters you found are used by users. Be sure to check that URL query parameters have not been excluded in the view setting

<!--EndFragment-->

### URL Parameter Tool in Google Search Console

Configure Google’s URL parameter tool to tell crawlers the purpose of your parameters and how you would like them to be handled.

<!--StartFragment-->

learn how to configure URL parameters in Google Search Console, rather than letting Googlebot decide.

<!--EndFragment-->

<!--StartFragment-->

use server-side URL rewrites to convert parameters into subfolder URLs.

<!--EndFragment-->