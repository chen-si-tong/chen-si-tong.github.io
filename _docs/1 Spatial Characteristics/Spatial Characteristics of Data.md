---
title: Spatial Characteristics of Data
category: 1 Spatial Characteristics
order: 1
---

Fire incidents are a growing concern for many cities, including San Francisco. Understanding the causes and patterns of these incidents is critical in developing strategies for prevention and mitigation. By analyzing past incidents and identifying high-risk areas, we can better allocate resources and take proactive measures to prevent future fires. 

we use K-means clustering to search centroids which means the red dots indicate the exact locations of the incidents from 2003-01-01 to 2019-12-31, and we can find which area we need to focus on.
This map shows that we divide the city into three parts and the number of fire incidents in the northeast part of the city is much higher than in other parts of the city


<embed 
       type="text/html" 
       src="/images/k-means_map.html"
       width="800"
       height="600"
       >    

we continue to focus on the northeast part of the city to find the tendency of longitude and latitude as time changes

<embed 
       type="text/html" 
       src="/images/two_lines_chart.html"
       width="800"
       height="600"
       >    

In conclusion we predict that the centroid will move toward bottom left in the map, and we inference that the number of fire incidents in the northeast part of the city near the next the centroid will increase.
