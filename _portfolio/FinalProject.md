---
title: "Final Project GES 486"
excerpt: "Project on the Loss of Farms in Maryland <br/><img src='/images/clagett-barns-with-sunflowers-roshani-kothari-1171x593.png'>"
collection: portfolio
---

<br/><img src='/images/farm.png'>

Introduction and Background
=====
I am investigating and mapping the decline of agriculture and loss of farms in Maryland, specifically due to development.
According to Preservation Maryland, if recent trends continue, Maryland stands to lose 178,000 acres of farmland by 
2040 – a whopping 8% – and 67% of that conversion will occur on Maryland’s Nationally Significant land. That 
is the equivalent of losing 1,400 farms, 144 millionUSD in farm output, and 3,200 jobs. I believe this to be an
extremely important issue for several reasons that are social, economic, and environmental.  Having farms and 
agricultural businesses is an important aspect of community.  Being able to know where food is coming from and 
supporting your neighbors helps bond people to their local area and encourage them to invest in their community.  
Agriculture is also a major source of small business and independent contractors, granting opportunities to skilled
workers outside of major corporations.  Economically agricultural is an essential part of the U.S. and plays a role
in Maryland’s economy. Agriculture is the largest commercial industry in Maryland, employing some 350,000 people,
including nearly 6,000 full-time farmers, and contributing some 8.25 billionUSD annually to the economy. Farms are
important for protecting the environment as well as helping to fight climate change. According to the 2017 annual
report of the Maryland Commission on Climate Change “land conservation and sustainable management offers an important
mechanism for mitigating and adapting to climate change [helping] to avoid or diminish additional GHG emissions which
would be associated with development”.   Areas designated for agriculture use are protected from development projects
which would otherwise clear vegetation and prevent soil infiltration.   Low density development such as suburban housing
developments are the greatest contributor to lost farmland and an unsustainable approach to human housing.


Methods and Results
======

To investigate this phenomenon, I used tools including RStudio and QGIS and acquired data from Maryland.gov, the US Census
Bureau, the USDA, and the USGS.  In the Census of Agriculture a farm is defined as farm “any place from which $1,000 or more
of agricultural products were produced and sold, or normally would have been sold, during the census year.”  

Maryland Land Use
=
The first map I wanted to look at was the Land Use Land Cover survey for Maryland to examine how our limited resources were 
being used.  


<br/><img src='/images/landuse.png'>

Maryland appears to be largely vegetated overall but in the urban areas there is almost no farms or forests. Notably, the areas
with much of the agricultural land, the farms are broken up by low density residential neighborhoods. 


NDVI
=
Next, I wanted to see if there was visible loss of agricultural land or vegetation in general due to the expansion of development.
To do this I acquired satellite images from the USGS around the greater Baltimore area to eastern shore region. The images were broken 
down into their individual color bands to calculate the vegetation index. Live green vegetation can be represented with the NIR and
Red Bands through the normalized difference vegetation index (NDVI) as chlorophyll reflects in the NIR wavelength, but absorbs in the 
Red wavelength.  I specifically chose to use images from August as this is when crops would be grown and appear green.


<br/><img src='/images/NDVI.png'>


Using this index, there appears to be little vegetation due to it being so broken up at the scale of satellite imaging.  Along the 
coasts are also densely populated and built up with residential houses. 


Farm Density
=
Using the Census of Agriculture from the USDA, I wanted to compare the number of farms to the number of people in each county where a 
farm is any place that produces and sells agricultural products.  This was related by classifying each county by the number of farms per 
square mile and containing a dot whose size corresponds to the number of people per square mile in that county. 


<br/><img src='/images/farmdensity.png'>



Developed Land vs Agricultural Land
=

The first map in this series shows the ratio of developed land to farm land in 1973 for each county on a color gradient from green to red 
with green having the least development.  


<br/><img src='/images/LU1973.png'>


The next map shows the ratio of developed land to farm land in 2010 for each county on a color gradient from green to red with green having
the least development.


<br/><img src='/images/LU2010.png'>

There has been a major shift in the use of land in Maryland favoring developers over farmers.


<br/><img src='/images/deltafarm.png'>

The last map in the series is the change in land use from 1973 to 2010 to highlight which counties are losing the most farmland






