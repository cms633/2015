---
layout: post
published: true
title: "Moby Dick: Path of Thoughts"
category: updates
author: Judy Chang
---

![Screen Shot 2015-03-11 at 6.24.50 PM.png]({{ site.github.url }}/assets/Screen Shot 2015-03-11 at 6.24.50 PM.png)
The markers on this map reflects every single location mentioned in the famous novel Moby Dick, everything from a place name someone said to a place the main characters have been to. Using Google Maps and Google Fusion Tables, we successfully mapped all these locations on the World Map. But if we were given flexibility to augment and modify this data, there are some changes that we hope to make.

First, we hope to make a distinction among location types. More specifically, for any place name mentioned, it can either simply mentioned as a place the main characters want to visit (e.g. "I want to go to Scotland"), a metaphor ("Go to Hell!"), or a place the characters at at right now ("We sailed through Spain"). If we are able to categorize these places, we can create a more specific map that illustrates the characters' journey. For example, taking all the places that they physically went in chronological order, we can construct the actual journey by connecting the locations in a path. Then for each physical location node, we can look at all the places that the characters mentioned while they are at that physical location, and draw an edge between that place and the place mentioned. Now we can imagine that certain places are mentioned more than others when the characters are in a certain place, and this can help us visualize the characters' though process.

Another idea would be a simple treemap that counts how many times each place is mentioned. This allow us to easily see which locations are mentioned more often than others, and also help us visualize the characters' journey.
