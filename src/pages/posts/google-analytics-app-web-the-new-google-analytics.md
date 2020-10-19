---
title: Google Analytics App+Web - The new Google Analytics
subtitle: Updated on 15th Oct 2020 as Google Analytics App+Web are out of beta
date: 2020-10-13T22:10:23.496Z
template: post
---
As on 14th Oct 2020, Google Analytics App+Web are out of beta. It known as Google Analytics 4.

Why 4? I think if you exclude Urchin, which was acquired by Google in April 2005, this is the 4th major iterations. 

![](/images/april-2005.png)

Introduce in July 2019, Google Analytics App+Web  data collection and analysis is based on the Event-Driven Data Model.  This model allows you to track *everything* as events, regardless of the platform - whether App or Web. Event-Driven Data Model itself is not new. Heap Analytics and Facebook Analytics are already in this Event-Driven Data Model of data collection. 

![A screenshots of the new Google Analytics dashboard ](/images/screenshot_2020-10-15-analytics-home.png "No more page view metrics. ")

## What Others Said

<!--StartFragment-->

I read all the blog post out there on Google Analytics 4 (GA4). Here my summary

- GA4 lets marketers understand what happens on their digital properties while respecting GDPR, ITP & user awareness about tracking and privacy
- The previous Acquisition Report in Google Analytics will split between User Acquisition (First Touch) and Traffic Acquisition. (the old Default Channel Grouping report). This the move from Channel focused ‘Last Touch Attribution’. 
- GA 4 do away the page view/screen view concept with a flexible system of events and parameters (aka event-driven data model). The event-driven data model works for websites and mobile apps
- 3 new metrics are introduced: Engaged Sessions” (in “Behavior” report), which removes bounces, “Engaged Sessions per User” and “Engagement Time”
- GA 4 comes with automatic event tagging for user scroll tracking, youtube video interactions, clicks to exit the site. (I used to provide value-add srrvices to code for event tagging)
- You can now use GA4 data with BigQuery without the USD 150,000 GA360. BigQuery, a Google Marketing Data warehouse opens up the availability to export raw, unsampled Google Analytics data. This allows business with advanced web analytics needs to integrating with CRM
- Google Data Studio has a direct connector into your GA4 property. No need to go through BigQuery to get your unsampled data into your data visualization tool

Here what [Search Engine Land](https://searchengineland.com/google-analytics-4-adds-new-integrations-with-ads-ai-powered-insights-and-predictions-342048?utm_source=testandoptimize.com&utm_medium=social&utm_campaign=split-test-2020) said abut the new Google Analytics

* New AI-powered insights and predictions
* Deeper audiences integration with Google Ads
* Customer lifecycle-framed reporting (my favourite)
* Codeless Event tracking
* More granular user data controls 

## BigQuery Export

A functional feature of Google Analytics App+Web is BigQuery Export. 

BigQuery export opens up the availability to export all the raw, unsampled Google Analytics data. This allows SME business deal with advanced Google Analytics needs like getting unsampled reports, connecting with reporting/visualization platforms or integrating with other datasets like your CRM

Previously, this BigQuery Export feature was only available in paid Google Analytics 360 (USD 150,000 per year).

## Data Sampling in Google Analytics

Google Analytics is a must have for every business in the beginning, but as your business grows you need more flexibility and customization, because Google Analytics may give you inaccurate data.

When your data is too large, instead of utilizing all of the data available, Google Analytics uses data sampling and shows you an incomplete traffic data set.

In data analysis, sampling is the practice of analyzing a subset of all data in order to uncover the meaningful information in the larger data set. Data sampling is a method and approach that available to Data analyst in their daily work.

## What about Google Analytics?

Google official line is

> We recommend continuing to use your existing Analytics properties alongside an App + Web property.

When I was hired for web analytics project, I always set up Google Analytics App+Web together with Google Analytics.

## Hire with Confidence

You can access and manipulate the data stored in Google BigQuery using Python and R. These 2 languages make it easier to build a statistical model which can be used for various purposes – understanding customers’ in-app behavior, predicting the churn rate, etc. I being up to speed with Google BigQuery since 2019. 

https://www.qwiklabs.com/public_profiles/fdf93c0d-bc8b-4952-b7fe-1dade1d6e917

https://www.coursera.org/account/accomplishments/specialization/PKU7C2X2QRG8