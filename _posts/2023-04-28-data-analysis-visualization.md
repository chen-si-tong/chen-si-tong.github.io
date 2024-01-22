---
title: Visualizations and Data Analysis 
type: major
---

The project is divided into three parts.

> The First Part - Exploring Spatial Characteristics of Data.

Firstly, Based on the attributes (longitude and latitude), we use K-means clustering to search centroids which means is the focus point of the fire. This algorithm works by dividing a set of data points into k clusters, where each point belongs to the cluster with the closest mean.	Putting the data of longitude and latitude into the map and marking the centroids, we can find which area we need to focus on.

The result is that we divide the city into three parts and the number of fire incidents in the northeast part of the city is much higher than in other parts of the city.

Secondly, we just focus on the northeast part of the city to find the  tendency of longitude and latitude as time changes.
In this part, we just use broken line graph showing the tendency directly.

* In conclusion we predict that the centroid will move toward bottom left in the map, and we inference that the number of fire incidents in the northeast part of the city near the next the centroid will increase.

<embed 
       type="text/html" 
       src="/images/JupyterNotebook/TheFirstPart.html"
       width="800"
       height="600"
       type= "application/x-ipynb+json"
       >   

> The Second Part - Exploring Temporal Characteristics of Data

In this part we also put our eyes on the northeast part of the city we plot the bar graph to present the amount of the fire incident in different year/months/hour/week, plot the line graph to show the amount of fire incidents by time period of the week because it is easy to find some trends, and plot the pie chart of ignition cause by classification in the northeast part to know the fraction of every ignition cause. (Ignition Cause: Unintentional/ Intentional/ Cause undetermined after investigation/ Failure of equipment or heat source/ Cause under investigation / Other /Act of nature)

* As for the trend of year, we can find that there are the largest fire incidents from 2007 to 2013, and in this period, there is a decreasing trend in the number of fire incidents. However, the amount of fire incidents decreases sharply in 2014.And we find [News](https://www.cbsnews.com/sanfrancisco/news/new-sf-budget-allows-for-hundreds-more-police-officers-firefighters/) explaining the result. 

* As for the trend of hour and week, we guess that the reason is people are much more active at around 8pm on the weekend especially Sunday and Monday than others, surging the amount of using household appliances or other things that lead to fire.

* As for pie chart we find ‘Unintentional’ is the most important reason to cause fire. And we decide to dig ‘Unintentional’more details.

<embed 
       type="text/html" 
       src="/images/JupyterNotebook/Thesecondpart.html"
       width="800"
       height="600"
       >  
    
> The Third Part - Exploring Association Rules of Data

We want know more about the ‘Unintentional’,so we use the Apriori algorithm to aggregate the attributes such as which attributes have the stronger relationship with ‘Unintentional.

Apriori algorithm is to discover frequent item sets from a given dataset. An itemset is a set of items that appear together in a transaction. Apriori support and confidence are two important measures used in association rule mining, which is a technique for discovering relationships between different items in a dataset.

we select some attributes(Item First Ignited, Ignition Cause, Action Taken Primary, Area of Fire Origin, Primary Situation,Hour) and discretize the them based on the clean data.

<embed 
       type="text/html" 
       src="/images/JupyterNotebook/P3cleanningdata.html"
       width="800"
       height="600"
       >  
    

The fist picture we plot is the Word cloud map. We can find the frequency of the words in the association rules.

<embed 
       type="text/html" 
       src="/images/JupyterNotebook/wordcloud.html"
       width="800"
       height="600"
       >  

The second picture is the bar chart, which means the support and the amount of different rules, and find the factors Investigate, Unintentional, Cooking fire, confined to container and Cooking area intertwine each others.

The third picture is scatter plot, in which we can see the distribution of confidence, and then we pick up some points that confidence is equal to 1, which means the factors behind the point must have strong relevance. 

<embed 
       type="text/html" 
       src="/images/JupyterNotebook/p3barandscotter.html"
       width="800"
       height="600"
       >  

The fourth picture is association rules network graph. Based on the confidence lager than 0.7, we can see the network among the different rules, making the relationship clearer.

<embed 
       type="text/html" 
       src="/images/JupyterNotebook/network.html"
       width="800"
       height="600"
       >  

* According to the pictures above, we conclude that watch out the appliances in the kitchen!!! When you do not use them, you had better to plug off. If you don’t do this, there is a high probability that kitchen appliances will overcharge and overheat, leading to a fire outbreak without people’s awareness.



