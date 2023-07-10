---
title: "Guide to moving to GA4 "
subtitle: Things to look out for when switching to Google Analytics 4
date: 2022-10-17T08:42:59.402Z
template: post
---
## C﻿heck List 
* Configure GA 4 as “Privacy Friendly as Possible"\
  <https://datatovalue.nl/google-analytics-4/privacy-settings/>
* Migrate your exclude referrals\
  <https://support.google.com/analytics/answer/10327750>
* Change Data Retentions From 2 Months to 14 Months so data is available when you make a YoY (year on year) comparison * \
  <https://support.google.com/analytics/answer/7667196?hl=en-GB&utm_id=ad>  
* Link GA4 to Adwords, Google Optimise & Merchant Centre
* Mark Goal Events as Conversions. In the left-hand navigation go to `Configure > Events`. Find the event you want to mark as a conversion in the ‘existing events’ table and toggle the button to mark them as a conversion.
* Exclude Internal Traffic - With GA4, it is a little bit more involved. There are 12 steps to do it compare to Universal Analytics (GA 3)
* T﻿rack site-search in GA4 - having **Enhanced Measurement** enabled is not going to work 

GA4 migration checklist from Google : <https://support.google.com/analytics/answer/10759417?hl=en>

## W﻿orth Noting

Features are not currently available in GA4 

1. Calculated Metrics
2. Annotations
3. Campaign Timeout
4. UTM Override
5. Exclude hostname filters  

\*﻿ On a separate note, the data retention period doesn’t apply to data stored in [BigQuery](https://support.google.com/analytics/answer/9358801?hl=en)  –  you can keep it forever there.

## Data collection settings that can be migrated

As long as your Universal Analytics property data collection is implemented in [gtag.js](https://www.testandoptimize.com/posts/use-tag-assistant-tool-to-verify-google-analytics-setup/) or Google Tag Manager

* [cookie customization](https://developers.google.com/analytics/devguides/collection/gtagjs/cookies-user-id)
* [ads personalization](https://developers.google.com/analytics/devguides/collection/gtagjs/display-features) 

Official Source: Analytics Help Center

## Dimensions and metrics differences

| Universal Analytics         | GA4                            |
| --------------------------- | ------------------------------ |
| `Average sessions duration` | `User engagement` / `Sessions` |
| `Conversion rate`           | `Conversions` / `Sessions`     |
| `Goal completions per user` | `Conversions` / `Total users`  |
| `Pages / Session`           | `Views` / `Sessions`           |
| `Value per Session`         | `Event value` / `Sessions`     |
| `Value per User`            | `Event value` / `Total users`  |



### **I want to** understand what traffic channels are most effective in driving conversions

Access the “Advertising” section in the left-hand navigation and then click on “Conversion paths”.

![](/images/screenshot-2022-10-21-193445.png)