---
title: Spatial Characteristics of Data
category: 1 Spatial Characteristics
order: 1
---

When we got the dataset of fire incidents in San Francisco, the things that came to our mind are that there are a number of factories and companies in San Francisco, and that as the famous tourist city, San Francisco has a large number of native residents as well as a large number of tourists. It indicates that there are many fire incidents in San Francisco. We want to figure out that the spatial distribution of fire incidents in San Francisco to find the place where the number of fire incidents happened. This map shows the spatial distribution of fire incidents.

<embed 
       type="text/html" 
       src="/images/k-means_map.html"
       width="800"
       height="600"
       >    
  
The red dots are the data that we put the all the fire incidents from 2003-01-01 to 2017-12-31 into the map and markers refers to cluster the points. We use different colors to distinguish different clusters of points, dividing San Francisco into **THREE** parts. We find that the number of fire incidents in the northeast part of the city is much higher than in other parts of the city, because the number of the blue markers with flag is more than the number of others.

Now let’s focus on the northeast part of the city to find out other things. Besides the spatial distribution, we also want to find that the tendency that as time changes, whether there is any change or pattern in the clustering of fire incidents, i.e., the areas where fires are most concentrated.

In the northeast part of the city, we pick up one of markers randomly. 
(blue icon with flag in the bottom left corner, when you put the mouse on it, it will shows the text ‘Centroids 1’)

<embed 
       type="text/html" 
       src="/images/two_lines_chart.html"
       width="800"
       height="600"
       >    


The two line chart based on the blue icon that we pick up record the changes of latitude and longitude from 2013 to 2017 respectively. We can find that the tendency of latitude toward to the low latitude. It shows that this icon will be shifted downwards next time, and that the tendency of longitude is little complexity that longitude toward the low longitude firstly and then go the high longitude. It shows that this icon will be shifted leftwards in the map next time. 

In conclusion we predict that the icon will move toward bottom left in the map, and we inference that the number of fire incidents in the northeast part of the city near the next icon we predict will increase. 


We have gained some spatial information about the occurrence of fire incidents. What does the temporal information look like?



