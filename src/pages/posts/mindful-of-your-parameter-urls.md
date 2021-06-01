---
title: Mindful of Your Parameter URLs
subtitle: URL Parameters are also known as a Query String or URL Variable. A URL
  Parameter is a set of values appended to a URL preceded with a question mark.
date: 2021-06-01T10:26:33.109Z
excerpt: URL Parameters are also known as a Query String or URL Variable. A URL
  Parameter is a set of values appended to a URL preceded with a question mark.
template: post
---
The most common types of URL parameters are:

* **Tracking** (UTM are common parameters for marketing campaigns) –  ?utm_medium=social, ?sessionid=123 or ?affiliateid=abc
* **Reordering** –  ?sort=lowest-price, ?order=highest-rated or ?so=newest
* **Filtering** –  ?type=widget, colour=blue or ?price-range=20-50
* **Identifying** – ?product=small-blue-widget, categoryid=124 or itemid=24AU
* **Paginating** – ?page=2, ?p=2 or viewItems=10-30
* **Searching** –  ?query=users-query, ?q=users-query or ?search=drop-down-option
* **Translating** – ?lang=fr, ?language=de or

### Problem with URL Parameters

Parameter URLs are all well and good until they’re hit by a ton of traffic and become a nuisance. This inundation of traffic can result in reports hundreds of pages long.  

If you know that certain parameter URLs should not be tracked,[ filter them out of your Google Analytics reports](https://www.searchdiscovery.com/blog/url-query-parameters-in-ga/).  

By filtering out parameter URLs where they make sense, you improve the accuracy of your tracking and create better attribution models for your search traffic.

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

### Plan of for SEO-friendly parameter handling

Jes Scholz, Group CMO at Ringier suggest the following approach:

* Do keyword research to understand what parameters should be search engine friendly, static URLs.
* Implement correct pagination handling with rel=”next & rel=”prev”.
* For all remaining parameter-based URLs, implement consistent ordering rules, which use keys only once and prevent empty values to limit the number of URLs.
* Add a rel=canonical link attribute to suitable parameter pages to combine ranking ability.
* Configure URL parameter handling in both Google and Bing as a failsafe to help search engines understand each parameter’s function.
* Double check that no parameter-based URLs are being submitted in the XML sitemap.