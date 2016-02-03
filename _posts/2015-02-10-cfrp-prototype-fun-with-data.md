---
layout: post
published: true
title: "CFRP Prototype - Fun With Data"
category: updates
author: "Yanni Coroneos, Corey Walsh"
---

## Collecting Data
Our idea hinges on the premise that we will be able to separate words and phrases. To this end, we could run the registers through an OCR algorithm and then run the textual output of that through a parser that correctly separates our text according to delimiters. For example, items on the registers are separated from their costs by commas or dots. The parser should know that the phrase/word on the left side of the dots is associated with the monetary value on the right. There are, of course, lots of edge cases where the specific dots example breaks down but the idea is correct.

## Data Contained In Registers
The registers are essentially a catalog of the costs that go into running the plays. The most important data they contain are seating positions and how many of those seats were sold. Additionally, they also contain auxiliary costs such as the price of the bottles of wine that the actors consumed and certain decorative embellishments such as a chandelier. Interestingly, the verbosity decreases with time.

## Data Storage and Presentation
Once the data is collected and indexed, it could be stored in either a relational or non-relational database. While non-relational is easier in implementation, relational databases such as SQL give a higher level of query access to the stored information. Once the backend was complete, it would open the gateway to building web-based interfaces, or even release a data-access API so that others could do the same.

The most important things in terms of presentation are:

1. Simplicity - if users can’t figure out how to interact with it, it’s not doing a very good job
2. Flexibility - a simple site isn’t very interesting if it can’t do anything

We propose building a small number of visualizations, that can be passed generic data models for display. On top of that, we recommend building a database query building UI that allows users to filter and select any data fields they so desire. This (if implemented correctly) accomplishes the second goal by removing limitations from the users’ access to data, and facilitates the first goal by logically reducing the problem to smaller pieces that can be individually optimized and streamlined by a programmer.

## Tools
The proposed model relies on having tools to accomplish the following tasks:

1. Building database queries
2. Displaying the result of those queries

There are multiple ways to implement these tools. For the first, we envision a system that takes a list of raw data, and and applies user specified transformations to that data to map or filter that raw data. One way to do this would be to let the user add to a list of ‘transformations’ that do pre-determined things. They might add a transformation that “Filters based on the price field for all records greater than 300,” or “Maps the output of this function to a new field called ‘profit.’” The application would have to simply sequentially apply the transformations that the user defined. Once the data pipeline is created, one must have some way of displaying that data, we propose two initial visualizations:

1. A line graph that allows for multiple lines
2. A heat map overlayed with the theater layout 

For the first, the user could define the x and y axis, and the data that should get graphed to each line. For the second, the system would just plot each data point based on seat location and build the heat map from the distribution of points.

## Audience
Our end product targets a wide audience. We think that historians and students could really use our website to get a feel for the era and even pick up on some specific facts. Additionally, actors could even use our website if they want to incorporate old styles into their current work/layout. It could also be neat if the actual Comédie-Française used our product as a distraction during intermission. The audience could play around with it while the scene changes.

## Questions Addressed
Our system allows for a large range of questions to be answered, limited primarily by the user’s imagination. Some example questions might include:

1. Most sought after seat for a given play
2. Most profitable wine selection
3. How world events impacted theater attendance

## Designs
![IMG_2254.JPG]({{ site.github.url }}/assets/IMG_2254.JPG)
