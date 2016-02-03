---
layout: post
published: true
title: Moby Dick Map
category: updates
author: hariharsubramanyam
---

I cleaned up the map we worked on in class and added some features.

The map occupies the full page now, which makes better use of the screen real-estate. The old version simply occupied a small part of the screen. Another change is that the map now loads points from the csv file, rather than from Fusion Table. The advantage here is that I can more easily hide/show points via the Google Maps API, and that the project is more self contained (it does not require access to Fusion Table).

I added the ability to search by quote. This way, you can look for similarities (ex. where do we see "Pine Barrens"). Another feature, which I didn't implement but would be useful, is searching by regular expression. This would give you much more power in your searchs.

I also allow the user to filter down to a specific range of sequence numbers. This is helpful if you're restricting your attention to a particular part of the book. I chose to use sequence numbers instead of page numbers because it required less cleaning, but using page numbers should be possible as well.

Finally, the user can animate the points. This is helpful to see how the focus of the story changes over time. Since dataset contains all referenced places, rather than the places that the story takes place in, the animation hops all over the globe. However, if we annotated the dataset to indicate the places that the story actually occurs in, then an animation might let us see the voyage.

Cleaning the data took some time, as did getting familiar with the Google Maps API. However, the features did not take too long to code. The website is still a bit slow, however.

See the website [here](https://mobydick.firebaseapp.com/ "moby dick")

![moby dick map]({{ site.github.url }}/assets/moby_dick_map.png)