---
title: "Sample Ratio Mismatch (SRM) in A/B Testing "
subtitle: What is it and what you can do about it
date: 2021-05-04T14:33:46.408Z
excerpt: What is it and what you can do about it
template: post
---
Some browsers and mobile devices could takes longer to load (~5 seconds) and affect A/B testing measurement.  If a test was configured to split traffic equally are not being observed,  there would be a Sample Ratio Mismatch (SRM). 

Similarly, if a test was configured to split traffic 80/20, there would be no Sample Ratio Mismatch detected if a 80/20 split is indeed observed.

There could be potential data quality issues on experimentation platforms such as

\- Google Optimize 

\- Omniconvert  

\- SiteGainer/Symplify 

\- Visual Website Optimizer (VWO)

Most testing platforms don’t alert users to SRM issues or even flag that their experiments are broken. This can change the outcomes of your experiments. 

A statistical method [goodness of fit](https://en.wikipedia.org/wiki/Goodness_of_fit) test to compute a p-value can be used.

At LinkedIn, **[about 10%](https://arxiv.org/abs/1808.00114)** of experiments suffer from sample ratio mismatch.

The authors of A Taxonomy and Rules of Thumb for Practitioners” ([link](https://dl.acm.org/citation.cfm?id=3330722)) provides several examples of causes of Sample Ratio Mismatch and offers 10 rules of thumb for quickly diagnosing and preventing SRM