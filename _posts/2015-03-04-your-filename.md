---
layout: post
published: true
title: Popularity and Success of Plays and Genres Over Time
category: updates
author: "Meghana Bhat, Judy Chang, Val Healy"
---

Our visualization: http://mit.edu/changycj/www/cfrp/cfrp.html

Our group decided to tackle the research question, how does the success and popularity of different genres and plays change over time? We decided to approach this question by looking at the number of performances of a genre/play in contrast to their ticket sales in different time spans. This visualization would aid research of French history and how events affected both the theatre and society. It could also be applied to current day, as we may be able to predict which genres or plays will sell more tickets--or possibly to figure out the optimal number of performances for getting ticket sales. We are starting with a small time span for our prototype, but we would stretch this to a larger number of years for the final version.

We initially envisioned that our visualization will look like the following:
![CFRPgroupmockup.png]({{ site.github.url }}/assets/CFRPgroupmockup.png)


The larger bubble graph would show either the number of performances or total ticket sales (based on the radio button selection on the side menu) for each genre over time. Different colors (and a color guide) would make it easy to identify the genre. The nested bubble graphs inside each bubble will show the same for each play. Hovering over a certain play bubble will give more stats on the play: the name of the play, total ticket sales, number of performances, etc.

We did have to deal with a lot of constraints in the making of our prototype, however. We used a tree graph because of issues with the d3plus library; we could not adjust the bubble sizes and distance between bubbles. The tree graph still gives a good idea of the relative popularity of certain plays and genres, though. We also had to limit the size of the data we were dealing with, both so that we could process it and so that it would not take forever to load. We decided to limit our data set to 12 quarters, 4 quarters in each of the years 1788, 1789, and 1790. Our visualization makes 12 different query calls, one for each quarter (changing the date=gte.YYYY-MM-DD&date=lt.YYYY-MM-DD accordingly), so that we have 12 queries running in parallel instead of making one gigantic query for 3 years. (This is one example API query to Postman: https://cfrp-api.herokuapp.com/play_ticket_sales?total_sold=gt.0&date=gte.1788-01-01&date=lt.1788-04-01 )