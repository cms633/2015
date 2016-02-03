---
layout: post
published: true
title: Map Update with Whale Populations
category: updates
author: Zach Sherin
---

For my update, I found a map of sperm whale populations and tried to overlay it onto the map. I ran into a few problems with this. First, the map had the pacific ocean in the center, which meant that overlaying it with the Google Maps API was surprisingly difficult, and I had to fix it in GIMP.
![map.jpg]({{ site.github.url }}/assets/map.jpg)
![spermwhalefixed.jpg]({{ site.github.url }}/assets/spermwhalefixed.jpg)
This was not that big a deal to fix, however, and was quickly (and mildly unprofessionally, sure) taken care of. The real problem was when I overlayed it on the actual map. At first look, it seems like there's no problem except for a slight mismatch in my latitude and longitude coordinates:
![updated map.png]({{ site.github.url }}/assets/updated map.png)

But then, if you look at other areas of the map, the problem becomes clear:
![mapproblems.png]({{ site.github.url }}/assets/mapproblems.png)

The map projections are different! This is something I would consider a major problem in any sort of geotagging experiment that involves the use of maps. The projection of the map matters enormously when trying to combine different maps, and mine was an incompatible projection.

The problem of projections is not unreasonable to solve. I could probably reproject the image onto a different map, or process the image to acquire the lat/long coordinates of the sperm whale grounds to be written directly onto the Google map. However, there is no easy tool to do this. I could write my own, but I feel that this reprojection problem should be solveable without cracking open an attempt at map reprojection software that I've never thought about before.

This is something I feel is a big problem with the mapping software: the different types of data (in this case, image overlays) have many different formats. Trying to overlay them all into a single map is potentially a daunting task, depending on the diversity of your data sources.