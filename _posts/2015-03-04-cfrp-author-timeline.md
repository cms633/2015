---
layout: post
published: true
title: CFRP Author Timeline
category: updates
author: "Harihar Subramanyam, Ariana Eisenstein, Sherry Ren"
---

### Research Question: Who were the authors of the Comédie-Française?

To answer our research question we have created a website mimicking the Internet Movie Database (IMDB), but instead of using actors, we used the playwrights of the CF. Each playwright and their work is catalogued to be searched and viewed quickly.

There will be two primary ways to search this database. First is a standard text-field search. A second option is to locate specific authors along the timeline displayed on the main page of the website. Each author is marked at their date of birth. Searching a specific year causes the timeline to display the span of ten-years from the query. This method helps contextualize the authors’ work by graphically showing the period in which they were alive, allowing the user to view which playwrights were contemporaries as well as understand the historical influences which  may have influenced their work. We found that initially the granularity of ten year periods resulted in an uncluttered visualization, which still displayed popularity trends, but that future iterations could include the option to change this scale. Additionally, we would include the ability to search plays as well as authors as well as the ability to scroll through the timeline. The initial mockup is shown below:

![mockup 1]({{ site.github.url }}/assets/timeline_mockup1.png)
![partb_timeline.png]({{ site.github.url }}/assets/partb_timeline.png)

After clicking on a specific author, the CF API is queried and the web page displays the authors lifespan, plays written, and total number of performances, which are pulled from the API and processed in real time.  The individual playwrights pages add more details such as the popularity of their work as well as their prolificness. It further contextualizes their work as it shown when the playwright was alive. A final iteration would show a graph detailing the number of tickets each type of ticket sold for each play, mapped against the year [Figure 2]. This graph will allow users to gauge which play was most popular and when it was playing. Outside sources of information, such as a link to the text of each play or a link to a biographical reference to each author, could be included on the individual author page as well. Another mockup is shown below:

![author page]({{ site.github.url }}/assets/author_page_mockup.png)
![partb_graph.png]({{ site.github.url }}/assets/partb_graph.png)


We implemented parts of the mockup in a website: [https://infinite-tor-5541.herokuapp.com/](https://infinite-tor-5541.herokuapp.com/). A screenshot of the website is shown below.

![timeline screenshot]({{ site.github.url }}/assets/author_timeline_screnshot.png)

When an author is selected (either by searching or clicking on timeline), their page appears (shown below).

![author page]({{ site.github.url }}/assets/author_page.png)

Authors appear multiple times in the dataset (ex. "Voltaire", "Voltaire (François-Marie Arouet dit )"), but our project corrects for this and retreives all plays for the given author and computes the total number of performances for the given author. The birthdate and deathdate were scraped from Wikipedia.

As the CF API grows, we believe this database could include data on actors and other people involved in the Comédie-Française. Thus, it will more closely resemble IMDB where each entry is connected to all others involved with it, leading to a more interconnected web of information. The one challenge with adding this data is to ensure that the visualizations do not become overcrowded and unreadable.

This website is designed for any person interested in French Playwrights and can be used with either little or vast amounts of previous knowledge. The interface is easy to use and highly intuitive. Considering inexperienced users, anyone curious about a specific playwright or a specific time period can quickly find the relevant information. As the data in the API grows, these users can gain intuition into the many interconnections between playwrights, plays, actors, and other principles of the Comédie-Française, resulting in the rabbit hole effect seen in websites like Wikipedia. Concerning more knowledgeable users, historians can use this database to see how the trends in French history effected specific playwrights writing. They can also view whether the work of later playwrights was influenced by the popular plays of their childhood or adolescence. Contextual questions of current trends influencing author’s works can be answered. Additional data can expand these questions past authors and examine the relations between actor or play and time period.