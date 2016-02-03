---
layout: post
published: true
title: "Averages and Sums, Success of Genres/Authors"
category: updates
author: Meghana Bhat
---

I ended up using IBM's ManyEyes for the visualization. I investigated the difference between the average and sum totals of the number of tickets sold based what genre the play was, and who the author of the play was. In class we had only looked at the sum totals, but I noticed that the comparison between the genres and authors looked a lot different when you looked at their average "success" instead (as measured by the number of tickets sold).

Consider, first, the following pie chart comparing the ticket sales of different genres:
![graph1.png NOT LOADING]({{ site.github.url }}/assets/graph1.png)
This shows that, in fact, tragedy/tragicomedy is the most successful genre on average. In contrast, consider the following pie chart on the sum of all ticket sales over the year for each genre:
![graph4.png NOT LOADING]({{ site.github.url }}/assets/graph4.png)
Comedy has by and large sold the most tickets over the course of the year. However, this is a deceptive number, as comedy had one of the lowest average ticket sales in the former graph! Thus, is comedy really the best genre? Perhaps people weren't as interested in comedies. Or perhaps there were so many comedies playing that people were no longer so inclined to see them. But why did the theatre keep playing pure comedies when other genres (such as tragedies) seemed to be more fruitful in ticket sales this year? 

In an attempt to investigate further, I looked at this box plot of the genres' ticket sales:
![graph5.png NOT LOADING]({{ site.github.url }}/assets/graph5.png)
This shows that comedies had a huge variance in ticket sales (the standard deviation is high). In comparison, tragicomedy, the genre with the highest average sales, seems to have just one data point! Perhaps the conclusion we could reach from the first graph was false--given more data points, tragedicomedies may not be the best bet of play to show. No, what would help may be some "weighted" average, where the genre's average lends bigger significance to the conclusion if there were more data points for that genre. We can still guess, though, from these graphs, that tragedies in general tend to have higher ticket sales during this year. Whether that means the theatre should have played more tragedies for higher profit, we cannot say.

I looked next at the authors' success, since the analysis was interesting for the genres. The following shows the average ticket sales of each author: (done in a bar graph for easier reading, since there are a lot more authors than genres)
![graph2.png NOT LOADING]({{ site.github.url }}/assets/graph2.png)
It looks like there are a few authors who have relatively abysmal ticket sales, and most authors seem to average around 400-500 tickets sold. However, Cahusac has significantly higher average ticket sales. But consider the total sold for each over the year:
![graph3.png NOT LOADING]({{ site.github.url }}/assets/graph3.png)
This time, Molilere takes the top position by a huge margin with 34 play performances. It turns out Cahusac just had one really good play performance. However, Molilere's plays' average ticket sales were a below-average 384. These were probably also, we can infer, the same comedies that had a high sum total of ticket sales.

The data suggests that Molilere's comedies were shown too often in this theatre. I wonder if they changed tactics for the next year, or if those comedies had been successful in the previous year for them to try them so avidly this year. More data points may reveal the answers.
