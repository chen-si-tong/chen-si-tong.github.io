---
title: Association Rules of Data
category: 3 Association Rules
order: 1
---

The aim of this part is to explore the association rules about Unintentional, which means according to the records in the dataset, find out which one attribute or several attributes can cause Unintentional. In other words, if we can know what can cause fire and the place that Unintentional happens more frequently, we can suggest people to be more care about these.

<embed 
       type="text/html" 
       src="/images/wordcloud1.png"
       width="800"
       height="600"
       >    


The picture above is Word cloud map, which represents the frequency of the words in the final association rules. We can see IFI76, IC2, ATP11, ATP86, AFO24, PS111, PS113, Hour4, Hour3. You can look the following table to check out the meaning of abbreviation.

| Abbreviation |       Full Name      | Abbreviation |                Full Name               |
|:------------:|:--------------------:|:------------:|:--------------------------------------:|
|      IFI     | Item First Ignited   |     IFI76    | Cooking materials, inc. Edible materil |
|      IC      | Ignition Cause       |      IC2     | Unintentional                          |
|      ATP     | Action Taken Primary |     ATP11    | Extinguish                             |
|      ATP     | Action Taken Primary |     ATP86    | Investigate                            |
|      AFO     | Area of Fire Origin  |     AFO24    | Cooking area, kitchen                  |
|      PS      | Primary Situation    |     PS111    | Building fire                          |
|      PS      | Primary Situation    |     PS113    | Cooking fire, confined to container    |
|              |                      |     Hour3    | 4AM - 6AM                              |
|              |                      |     Hour4    | 6AM - 8AM                              |

The following picture reveals that the number of association rules and the support of each association rules. we can find (ATP86),(ATP86,IC2),( ATP86,IC2,PS113), ( ATP86,IC2,PS113,AFO24) is the highest respectively. It sounds like so complex but
in another word, there are some relationships among Investigate, Unintentional, Cooking fire, confined to container and Cooking area.

<embed 
       type="text/html" 
       src="/images/apriori_bar.html"
       width="800"
       height="600"
       >    

Now we know that the factors Investigate, Unintentional, Cooking fire, confined to container and Cooking area intertwine each others, but what is the specific rule? we can read the scatter plot as follow.

<embed 
       type="text/html" 
       src="/images/apriori.html"
       width="800"
       height="600"
       >    

The pictures show that there are many points when confidence is equal to 1, which means the factors behind the point must have strong relevance. Next, we pick up these points. The following table show these points.

<embed 
       type="text/html" 
       src="/images/apriori_table.html"
       width="800"
       height="600"
       >    

From the table, the period between 4am and 8am in the morning is the most prone time for ‘Unintentional’ fires to occur, and most of the ‘Unintentional’ take place on the cooking area.

If confidence is not equal to 1,we make confidence lager than 0.7, we will draw the association rules network graph and see the more association rules than before.S

<embed 
       type="text/html" 
       src="/images/networkx_plotly.html"
       width="800"
       height="600"
       >    

Until now I think we can conclude something. Watch out the appliances in the kitchen!!! When you do not use them, you had better to plug off. 
If you don't do this, there is a high probability that kitchen appliances will overcharge and overheat, leading to a fire outbreak without people's awareness.

