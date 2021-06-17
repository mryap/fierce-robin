---
title: Extract, Transform and Load on Google Cloud Platform
date: 2021-06-17T11:46:49.503Z
template: post
---
I try to get a sense of different cloud computing tools on Google Cloud Platform (GCP) that brings data from disparate sources together, transform and enhanced it in a useful way ( beyond removing Not Available, Null data) to finally store and analysis in BigQuery. The process is known as ETL (Extract, Transform and Load)

Tyler Treat gives the big pictures on several options when it comes to implementing ETL processes on GCP options. His article helps as I am familiar with GCP and Google BigQuery. 

Anyway, here the gist:

* For low/no-code solutions, Data Fusion and Cloud Dataprep are your only real options.

* Dataprep is more refined and cost-effective but limited in capability, and it brings a [third-party vendor (Trifacta)](https://cloud.google.com/dataprep) into the mix.  

* For teams with a strong engineering background, recommended starting point is Cloud Dataflow or even Cloud Tasks 

Lastly my favorite, BigQuery itself for ELT is also an option for SQL-minded teams.

### BigQuery

In Tyler words 

' BigQuery provides a good mechanism for ELT — that is extracting the data from its sources, loading it into BigQuery, and then performing the transformations on it. This is a good option if you’re dealing with primarily batch-driven processes and you have a SQL-heavy team as the transformations are expressed purely through SQL. The transformation queries can either be scheduled directly in BigQuery or triggered in an automated way using the API, such as running the transformations after data loading completes.'


![image](https://user-images.githubusercontent.com/15719191/122387584-ea553a80-cf66-11eb-85a6-39be39ad353b.png)
