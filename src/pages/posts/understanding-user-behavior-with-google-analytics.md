---
title: Understanding User Behavior with Google Analytics
date: 2020-07-01T13:02:13.015Z
template: post
---
<!--StartFragment-->

As a business, it’s critical to understand how people use your applications, including mobile apps (iOS and Android), web and SaaS applications, and IOT (internet of things) devices. Understanding user behavior helps you improve the user experience, refine features and content, and build a product that is useful to your users. 

Google Analytics can help you measure user behavior, find insights about usage, and drive real change that improves the user experience and your business performance. 

The more you know about your users, the better equipped you’ll be to make informed choices.

<!--StartFragment-->

Google Analytics provides many pieces of information to help you understand the behavior of users as they interact with your site or application. Standard metrics include 

* the number of users interacting with your application
* the number of sessions those users create, and 
* the screens or web pages that they visit

<!--EndFragment-->

<!--StartFragment-->

With additional set-up, you can gain an even richer understanding of how people interact with individual application screens or pages on a website. You can capture more detailed interactions where needed using event tracking for granular interactions like those with video players, downloads, form submission, etc. You can also measure the number of important business actions that users complete (called Goal Conversions), as well as ecommerce transactions and purchases.

<!--EndFragment-->

<!--StartFragment-->

## Measurement planning

Every business should create a measurement plan to guide their analytics implementation. This helps you focus on the data related to your business-measurement needs that tied in with your business models. Collecting every user interaction can create a data set that is too large and difficult to analyze.

Your measurement plan should define:

* Overall business objectives
* Strategies and tactics that support the overall business objectives
* Key performance indicators (KPIs) to measure the success of strategies and tactics
* Segments to better understand what drives success -- this includes segmenting marketing activities and your most valuable users
* Targets for each KPI to understand if your business is reaching its goals

To gather this information, take the time to discuss your business objectives with those people in your organization that will be using the data. This might include product designers, marketers, and others that make business decisions. You want to understand the critical pieces of information that will help people understand the performance of their business. Document their answers and create a simple measurement plan.

<!--EndFragment-->

<!--StartFragment-->

### Goals

Goals measure how effectively your application or website supports your business objectives. A goal represents a completed activity, called a conversion, that contributes to the success of your business. Examples of goals include 

* purchase transactions (for an ecommerce business),
* game-level completions (for a mobile gaming app),
* submitting a “contact me” form (for a marketing or lead generation site), or
* using a specific feature within your SaaS application.

Defining goals is a fundamental component of any digital analytics measurement plan. Having properly configured goals allows Analytics to provide you with critical information to better understand if users are completing the behaviors you want them to complete. Without this information, it's almost impossible to evaluate the effectiveness of your online business.

<!--StartFragment-->

Pro-tips: Goals in Google Analytics only start showing data once you have configured them. So, if you forget to set them up, this will happen.

![](/images/d1pgui5xqakur5j.jpg)



<!--EndFragment-->

<!--EndFragment-->

## Enhanced Ecommerce

Enhanced Ecommerce tracking allows you to measure the number of transactions and the revenue that your website or mobile app generates. Enhanced Ecommerce tracking helps you understand user behavior across the user's entire online shopping experience including: 

* product impressions, 
* product clicks, 
* viewing product details, 
* adding a product to a shopping cart, 
* initiating the checkout process, 
* transactions, and 
* refunds

![Enhanced eCommerce in Google Analytics helps you obtain reports such as Purchase Funnel Analysis (where people abandon), Checkout Behavior (how they are moving from a step to another), Product Performance (add-to-cart rate, buy-to-detail rate, removes from the cart)](/images/eyw_-fzwaaesv6q.png)

## Event Tracking

Events are user interactions that are tracked independently from a web-page load or screen load. You can use events to track interactions within application screens or web pages. Events are commonly used in mobile apps to understand how users share content with other users, how they use the app’s search function, and when they select specific pieces of content. Events are commonly used on websites to track file downloads, content shares, and gadget interactions. Events are extremely flexible and let you collect the data you need to better understand user behavior.

## Custom Dimensions & Metrics

Custom dimensions and custom metrics are like default dimensions and metrics in your Analytics account, except you create them yourself! You can use them to collect and analyze data that Analytics doesn't automatically collect. For example, you might use a custom dimension to collect the user’s level in a mobile-app game. Or, if you’re a publisher, you might use a custom dimension to collect the user’s subscription level. Custom dimensions and metrics let you combine Analytics data with non-Analytics data, providing deeper insights into user behavior.

## Reporting

Now that we’ve discussed some of the most common implementation customizations, let’s look at the actual data. Below are a number of analysis techniques that can help you gain insights into user behavior.

### Active Users

Like any business, you want to keep track of the level of user interest. If the numbers are consistently in line with your expectations, you’ve found your sweet spot.

If the numbers are below expectations, re-evaluate your marketing efforts to see whether you’re targeting the appropriate audiences, and whether your ads are winning auctions. You can also look for any negative press or social content that might affect traffic. Even if all the marketing and social buzz are positive, you may be creating technical hurdles for your users with your site or app design.

In cases where you have a lot of 1-Day Active Users but the numbers drop off for longer term users, that can signal things like problems with a new release, or that initial enthusiasm isn't translating into long-term engagement. For example, many users might be downloading an app but finding that it doesn't meet a need they have or that it doesn't capture their interest.

## Cohorts

A very common way to measure user engagement is through a technique called cohort analysis. A cohort is a group of users who share a common characteristic. For example, all users with the same Acquisition Date (or first use) belong to the same cohort. The Cohort Analysis report lets you isolate and analyze cohort behavior.

Cohort analysis helps you understand the behavior of component groups of users apart from your user population as a whole. For example, you can use cohort analysis to:

* Examine individual cohorts to gauge response to short-term marketing efforts like emails or notifications to users.
* See how the behavior and performance of individual groups of users changes day to day, week to week, and month to month, relative to when you acquired those users.
* Organize users into groups based on shared characteristics such as Acquisition Date, and then examine the behavior of those groups according to metrics like User Retention or Revenue.

Understanding the point at which users tend to disengage (for example, initiate fewer sessions, view fewer pages, generate less revenue) can help you identify two things:

* Common points of attrition that might be easily remedied
* The rate at which you need to acquire new users to compensate for unavoidable attrition

## Behavior Flow Report

The Behavior Flow report visualizes the paths users traveled from one screen, page or event to the next. This report can help you discover what content keeps users engaged with your site. The Behavior Flow report can also help identify potential content or usability issues.

Use the Behavior Flow report to investigate how engaged users are with your content and to identify potential content issues. The Behavior Flow can answer questions like:

* Is there an event that is always triggered first? Does it lead users to more events or other behaviors?
* Are there paths through your mobile app or site that are more popular than others, and if so, are those the paths that you want users to follow?
* Did users go right from product pages to checkout without any additional shopping?

## Event reporting

Event reports organize your events into Category, Action, and Label. The specific categories, actions and labels that the reports display reflect the taxonomy that you have created in your event tracking code. For example, to track interactions with your video player, you might set up the following categories, actions, and labels:

```
Category: “Videos: Instructional”, “Videos: Music”
Action: “Play”, “Stop”, “Pause”
Label: “Dance music video”, “Getting started with Google Analytics”
```

## Custom Dimension & Metric reporting

Once you have configured and collected custom dimensions and metrics, they become available via the user reporting interface. Custom dimensions and metrics are available in custom reports, and are available for use with advanced segments. Custom dimensions can also be used as secondary dimensions in standard reports.

For example, you might use custom dimensions and metrics to learn about player behavior in a gaming app. Using custom dimensions, you could create new groupings of hits, sessions, and users. Additionally, you might want to sell extra features to enhance the user experience, such as "powerups". You could use an extra field to measure the strength of each powerup that users purchased. This way, you’d be able to determine if certain powerup strengths were more popular than others. Using custom dimensions and metrics in this way would allow you to answer questions like:

* How many times are easy levels played versus medium or hard levels?
* How many levels are played for each day in a 3-day free trial?
* How many levels are played by users in the trial versus users who have paid for the game?

Understanding how Google Analytics creates its standard reports or custom tables, it’s necessary to understand [how scope affects which dimensions and metrics are in each report](https://support.google.com/analytics/answer/1033861?hl=en).

<!--EndFragment-->