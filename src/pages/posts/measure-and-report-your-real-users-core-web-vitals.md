---
title: "Measure and report your real-users Core Web Vitals "
date: 2021-04-23T07:27:14.486Z
template: post
---
Website site owners can measure the quality of their site’s user experience with a set of metrics called *Core Web Vitals.*

It serve as a proxies to measure the quality of a site’s user experience. They are Largest ContentFul Paint (loading), First Input Delay (interactivity) and Cumulative Layout Shift (visual stability). Here the thresholds websites need to meet.



![](https://13abu1tovy91hmtpm1t25cse-wpengine.netdna-ssl.com/wp-content/uploads/core-web-vitals.jpg "Image from the Google Search Central blog")

Google has announced that Core Web Vitals will become a ranking factor as of mid-June 2021.  

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

\- you should be able to view the web page's Core Web Vitals in the Top Events report in Analytics as you see in this screenshot:

![Web page's Core Web Vitals in the Top Events report in Analytics](/images/screenshot_2021-04-23-measure-and-report-core-web-vitals-with-the-web-vitals-library.png)