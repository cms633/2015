---
layout: post
published: true
title: That Pulsar Thing
category: updates
author: The Data Guzzlers
---

Here is the link to our CFPR Pulsar Finder: [roslin.mit.edu:2000](roslin.mit.edu:2000)

We decided to continue on with the use of Pulsar finders. Pulsar finding finds patterns as they appear over time (canceling out the noise and irrelevant outliers). In one of the first classes in CMS.633, we talked about clustering algorithms used to find correlations. Our pulsar finder does indeed find interesting correlations over time. 

Our visualization shows the strong effects of day of the week, month, year, and decades on all other parameters (genre, title, and author). As a tool for historians, we decided to focus on chronology because the work of the CFRP lasts over a very long period of time.

Design changes:
We used some simple CSS to edit the input and submit fields. However, the meat of our visual design is provided by the library Chart.js, so the more meaningful design changes would be creating meaningful x and y axis labels as well as point labels. We would also abstract away the way we search the API for information and provide more intuitive verbs. In addition, we would seek to compare to data sets as visualized below.

![Two Data Sets Example]({{ site.github.url }}/assets/comparing_two_datasets.png)

