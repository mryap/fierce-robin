---
title: "Measure and report your real-users Core Web Vitals "
subtitle: Google has announced that Core Web Vitals will become a ranking factor
  as of mid-June 2021.
date: 2021-04-23T07:27:14.486Z
thumb_img_path: /images/e0ekjttxoaimzin.png
img_path: ""
excerpt: Traditional site speed metrics alone don’t always tell the whole story
  of page load. Core Web Vitals offers a more nuanced metrics that can help to
  tell how users actually perceive the loading of a page.
template: post
---
Website site owners can measure the quality of their site’s user experience with a set of metrics called *Core Web Vitals.*

It serve as a proxies to measure the quality of a site’s user experience. They are Largest ContentFul Paint (loading), First Input Delay (interactivity) and Cumulative Layout Shift (visual stability). 

![](https://13abu1tovy91hmtpm1t25cse-wpengine.netdna-ssl.com/wp-content/uploads/core-web-vitals.jpg "Image from the Google Search Central blog")

You can access these metrics within Google Search Console at https://search.google.com/search-console/core-web-vitals/

![](/images/screenshot_2021-04-28-core-web-vitals.png)

<!--EndFragment-->

**Incorporate core web vitals into Google Analytics.**

<!--StartFragment-->

Google has begun to incorporate these metrics into a variety of different tools such as [Page Insights](https://developers.google.com/speed/pagespeed/insights/) and Search Console.  The [Page Insights](https://developers.google.com/speed/pagespeed/insights/) tool provides results  based on software checks. Collecting vitals from real users provides data “in the field” which can be more relevant

Sending these metrics to Google Analytics using the [web-vitals JavaScript library](https://github.com/GoogleChrome/web-vitals/) is straight forward. Note that capturing web vitals will only work on Chromium-based browsers (for the most part) as described [here](https://github.com/GoogleChrome/web-vitals/#browser-support).

<!--EndFragment-->

\- Add the web-vitals library to a web page

```
<script type="module">
  import {getCLS, getFID, getLCP} from 'https://unpkg.com/web-vitals?module';

  getCLS(console.log);
  getFID(console.log);
  getLCP(console.log);
</script>
```

\- Copy this, which sends the Core Web Vitals to Analytics.

```
function sendToGoogleAnalytics({name, delta, id}) {
  // Assumes the global `gtag()` function exists, see:
  // https://developers.google.com/analytics/devguides/collection/gtagjs
  gtag('event', name, {
    event_category: 'Web Vitals',
    // Google Analytics metrics must be integers, so the value is rounded.
    // For CLS the value is first multiplied by 1000 for greater precision
    // (note: increase the multiplier for greater precision if needed).
    value: Math.round(name === 'CLS' ? delta * 1000 : delta),
    // The `id` value will be unique to the current page load. When sending
    // multiple values from the same page (e.g. for CLS), Google Analytics can
    // compute a total by grouping on this ID (note: requires `eventLabel` to
    // be a dimension in your report).
    event_label: id,
    // Use a non-interaction event to avoid affecting bounce rate.
    non_interaction: true,
  });
}

getCLS(sendToGoogleAnalytics);
getFID(sendToGoogleAnalytics);
getLCP(sendToGoogleAnalytics);
```

\- You should be able to view the web page's Core Web Vitals in the Top Events report in Analytics as you see in this screenshot:

![Web page's Core Web Vitals in the Top Events report in Analytics](/images/screenshot_2021-04-23-measure-and-report-core-web-vitals-with-the-web-vitals-library.png)

Here the thresholds websites need to meet. 

![](/images/e0ekjttxoaimzin.png)

Mobile and desktop scores may differ significantly. It being recommend to run separate audits for desktop and mobile.

According to research by Akamai, users expect websites to load in 3 seconds or less. It helps to keep an eye on these 3 core web metrics vitals. Now you can incorporate these new more nuanced metrics in Google Analytics that can help to tell how users actually perceive the loading of a page.

If you want to send the Core Web Vitals metrics to Google Analytics using Google Tag Manager, please [contact me](https://www.testandoptimize.com/contact)

<!--EndFragment-->