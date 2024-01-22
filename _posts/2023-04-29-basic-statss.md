---
title: Basic Stats
type: major
---

> Data Cleaning 

Because some of data in the fire incidents dataset are NAN, we remove them from the datasets, and then we pick up 13 attributes that are relative to the major factors of fire incidents. Next we filtrate the time of fire incidents from 2003-01-01 to 2017-12-31. After cleaning, there is 25924 rows × 13 columns.

<embed 
       type="text/html" 
       src="/images/JupyterNotebook/DataCleaning.html"
       width="800"
       height="600"
       >   

>Data preprocessing

After cleaning data, we find that we can not use the data directly because the numbers were mixed up with the instructions in the same cell. We extract serial number, extract the date of year/month/hour, and split the longitudes and latitude.

<embed 
       type="text/html" 
       src="/images/JupyterNotebook/Datapreprocessing.html"
       width="800"
       height="600"
       >   

>Dataset Stats

We not only cope with data in descriptive statistical analysis, but also calculate the coefficient of association between each two attributes and draw the plot of it. We find that the coefficient of association between each two attributes is low (smaller than 0.01).
We also plot the boxplot to detect the outlier. we find that attributes of ‘Suppression Personnel Primary’,‘Situation_number’, ‘Ignition Cause_number’, ‘longitude’have outliers. The first three attributes are discrete attributes. We ignore them.
We also ignore because according to our aim, we just analyze the place in northeast of San Francisco.

<embed 
       type="text/html" 
       src="/images/JupyterNotebook/Datasetstats.html"
       width="800"
       height="600"
       >   