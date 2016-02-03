---
layout: post
published: true
title: CFRP Prototype
category: updates
author: Ariana Eisenstein
---

In developing the CFRP prototype, I was inspired by the "Mapping the Republic of Letters" project. I believe this project conveyed a large amount of data in an intuitive fashion, while maintaining the ability to easily pinpoint details. Thus, my prototype connects the audience class and size, play, and time period in an attempt to convey broad societal trends in Paris and France as a whole, to promote a distant reading of the data. In addition, the prototype will be easily searchable through these categories to allow for closer reads as necessary. In this manner, both scholars and students, familiar and unfamiliar with the topics explored will be able to gain a meaningful understanding of the themes explored.

## Data Extraction
For most of the history of the Comédie-Française, records of play attendance and revenue have been kept by hand. Thus, in order to extract meaningful data these records must be digitized. Several methods will be employed to complete this task.
First we will use computer-vision tools, such as LeNet-5 [http://yann.lecun.com/exdb/lenet/index.html] to segment the words and numbers and attempt to parse them into digital versions. These initial attempts will need to be augmented to identify any words and numbers that could not be identified by the parser. For this mostly likely captchas and expert review will be used.

## Data Presentation
The prototype will present the data in the form of a timeline on which represents all the days the theatre has been open. For readability, users will be able to select a span of years, and the timeline of the years, with a separate timeline for each year, will be displayed (see attached picture). From these timelines, graphs would be displayed showing the number of tickets sold of each type as well as include a hyperlink to an article on the play. Using historical data on where the CFR was currently located, different colors would be used to differentiate between the locations of the theatres showing the plays. Users can isolate certain ticket types to see when they occur most frequently. A scrolling bar of al the years will allow for users to quickly move between timelines.

## Audience
The audience for this prototype will be researchers and students attempting to gain insight into into trends or snapshots into specific periods of French history. The intuitive interface should allow those without in depth knowledge of the time period to observe trends in French society. Simultaneously, scholars with in depth knowledge of the time period will be able to perform both broad and close reads of the data, while maintain coherent links between the individual details.

## Research Questions
As mentioned above the questions that this work addresses involve the intersection between time period, attendee types, location, and play. Specifically, what types of plays appealed to specific demographics? Did these relations shift over time? Is there a relation between viewing population and location? This prototype would allow researchers to examine the connections between these factors.

## Prototype Design
![prototype.png]({{ site.github.url }}/assets/prototype.png)

