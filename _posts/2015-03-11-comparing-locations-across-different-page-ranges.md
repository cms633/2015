---
layout: post
published: true
title: Comparing locations across different page ranges
category: updates
author: Ben Reynolds
---

For my data mapping project, I created webpage that visualizes the locations in Moby Dick based on page ranges. Given a start page and an end page, you can filter down the results displayed on the map so that only references from the desired pages appear.

You can view a demo of the webpage [here](https://rawgit.com/Benolds/CMS-633-Moby-Dick-Locations-Visualization/master/showMap.html)

I decided that this tool on its own is limiting, but becomes much more powerful if you have an easy way to compare the resulting references to those of another page range. Thus, I added another layer to the map that uses a different pin color. You can now enter two page ranges; one for the first layer, and one for the second layer, and see the results on top of one another for easy comparison.

Here is a screenshot of the interface:

![Screen Shot 2015-03-11 at 4.27.49 PM.png]({{ site.github.url }}/assets/Screen Shot 2015-03-11 at 4.27.49 PM.png)

The red markers display the first layer, which in this case represents all the locations mentioned in the first 50 pages of Moby Dick. The blue markers display the second layer, which represent the _last_ 50 pages in this example. It's interesting to see the difference between the locations mentioned in the beginning, versus those mentioned at the end of this novel. For example, this visualization makes it clear that there are many more references to Western Europe in the beginning of the book than there are at the end.