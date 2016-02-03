---
layout: post
published: true
title: MuRoam Updates
category: updates
---

powerpoint link: https://docs.google.com/presentation/d/1lfWwxOdCzc3zUUHZ-A7djCxrPDOFi8XlHHSuyg8EkiA/edit#slide=id.gae980478f_0_0

Thanks to the help of the Artbot team (Desi Gonzalez and Liam Andrew) we were able to come across many resources and readings on location based apps designated specifically for museums.

The [first paper](http://mw2015.museumsandtheweb.com/paper/location-location-location-the-proliferation-of-indoor-positioning-and-what-it-means-and-doesnt-mean-for-museums/) by Matthew Tarr from the American Museum of Natural History, was about indoor location tracking technologies and its implications for museums. Tarr made some very important points on the limitation of current indoor positioning systems (IPSs), which cannot be achieved via traditional GPS methods. Many large-scale companies (like Apple and Google) are now working on solving this problem, but as of yet, “there isn’t a standout winner”. We were personally restricted by this technological limitation when our most promising IPS IndoorAtlas failed to properly calibrate in the large rooms of the MFA.

However, other points in Tarr’s paper, along with [a project from the Metropolitan Museum](http://www.metmuseum.org/about-the-museum/museum-departments/office-of-the-director/digital-media-department/digital-underground/2014/accessible-wayfinding) was essential in providing us with new direction for MuRoam. The project for the Met, designed by an Intern at the Metropolitan Media Lab, is a “path generator”, that allows users to pick paths through the museum based on illumination, crowdedness and loudness of rooms. However, this automated path generator also comes with a HTML based toolkit that allows users to draw their own paths on any floorplan in the form of lines and nodes, and upload these maps in the form of a JSON file. This tool is extremely beneficial for us, as we hope to use it in our design.

So to keep our approach realistic for the span of this class, we will go about the “draw-your-path-as-you-go” approach for MuRoam. Users will draw their paths as they walk around the museum, double tapping at location where they wish to drop pins. With the pins, we not only hope to encode a pausing point by the visitor, but also other important metadata, such as user orientation (which direction is the person facing), wait duration, and annotations. We realize that this is not the most ideal approach, but given our current restrictions and resources, it is feasible.  We want to design our app such that it is flexible for the potential implementation of IPS in the future.

We have had the opportunity to experiment and create beta versions of our technology. We developed a mobile site that holds a lot of the functionality we envisioned our application having.

![Screen Shot 2015-04-22 at 12.52.55 PM.png]({{ site.github.url }}/assets/Screen Shot 2015-04-22 at 12.52.55 PM.png)

One of the pages contains the current exhibits with user ratings. Upon reading/visiting the description of the exhibit, the user has the ability to leave a rating, which we believe is a simple yet powerful form of user participation.

![Screen Shot 2015-04-22 at 12.53.23 PM.png]({{ site.github.url }}/assets/Screen Shot 2015-04-22 at 12.53.23 PM.png)
![Screen Shot 2015-04-22 at 12.53.41 PM.png]({{ site.github.url }}/assets/Screen Shot 2015-04-22 at 12.53.41 PM.png)

Additionally, we have a section for drawing paths. On this page, users have the ability to upload paths they created and view other user created paths.

![Screen Shot 2015-04-22 at 12.53.08 PM.png]({{ site.github.url }}/assets/Screen Shot 2015-04-22 at 12.53.08 PM.png)


Implementing our iOS application has proved to be a challenge, at this time we will work on developing polished mockups of our application, but keep the functionality in the website. We now hope to add the augmentations mentioned above (direction encoding by replacing node circles with arrows, encoding of wait durations via node size) to the path drawing page weithin the next couple of weeks. Finally, we will be thinking of ways to make our app a better participatory tool by thinking of ways to make the interface more user-friendly and intuitive.