---
title: Melbourne Bicycle Traffic
subtitle: How has the Covid-19 pandemic changed our cycling habits? Let’s see.

date: 2021-11-13 00:00:00
description: Analysis of Melbourne bicycle traffic using open data

featured_image: '../Sensor_Site_Map.png'
accent_color: '#4C60E6'
gallery_images:
  - '../../visuals/bicycle_flows/Map snip-01.svg'
---

#### The data

This analysis uses [open data](https://discover.data.vic.gov.au/dataset/bicycle-volume-and-speed) and open software to investigate Melbourne’s bicycle traffic across the last four years. 

Melbourne bicycle volume and speed are recorded by sensors at 42 off-road and 4 on-road counter sites. Most sites have two sensors embedded in the pavement to measure bi-directional bicycle traffic.

The dataset includes information such as the volume of cyclists crossing the sensor, their speed, the gap between cyclists, as well as measurements on the wheelbase and axles which indicate the type of bike being ridden.


<br>

###### Bicycle Sensor Map (Jan 2018 - Oct 2021)

<!-- The map below shows the **location**, and **monthly average speed** and **number of cyclists** from Jan 2018 - Oct 2021. -->

*Hover on the map to view the monthly total of cyclists and their average speed.*
<iframe src="/data_stories/visuals/bicycle_flows/Sensor_Map.html" class="video-wrap full-width" height="600px"  style="border:none;"></iframe>

#### Annual bicycle traffic
<br>

Across the four years there were 46 million bicycles registered by the network of sensors across Melbourne. For convenience we'll refer to each bicycle registered by a sensor as a cyclist. 

If we breakdown the total volume of cyclists measured by each sensor, we can see that some sensors experience a much higher traffic than others, with a range from 26 thousand to 2.8 million cyclists recorded. 

<br>

###### Bicycle volume by sensor
*Scroll to see the complete list, hover to view percentage*[^1]

<iframe src="/data_stories/visuals/bicycle_flows/Sensor_by_volume.html" class="video-wrap full-width" height="400px"  style="border:none;"></iframe>
<br>

#### 2020/2021 : Bushfires & a global pandemic
2020 and 2021 were extraordinary years.  From late 2019, Victoria was affected by [devastating bush fires](https://www.vic.gov.au/2019-20-eastern-victorian-bushfires) with a State of Disaster declared on 2 January 2020.  Health warnings were issued due to smoke, with Melbourne's [air quality](https://www.theguardian.com/australia-news/2020/jan/14/melbourne-choked-by-hazardous-smoke-as-bushfires-continue-to-burn-across-victoria) described as the 'worst in the world' in mid-January. 

From March 2020 and through 2021, Melbourne enacted a broad range of [public health measures](https://www.dhhs.vic.gov.au/coronavirus-update-victoria-26-march-2020) to curb the spread of Covid-19. These restrictions included density limitations in public spaces, the donning of masks outside the home, and measures aimed at minimising population mobility. 

The impact of these events is reflected in the bicycle traffic data. 

Shifts in the volume, speed, direction, and location of bicycle traffic show that patterns of how and where people cycle changed in the 2020-21 period. Combined with the context of public health measures, these shifts are indications of how cycling behaviour was affected by wider social factors. 
 

#### Volume
<br>

<!-- We aggregated the bicycle sensor data at monthly and weekly intervals for analysis of cycling trends. -->

<!--  taking the count of cyclists and their average speed by key attributes like direction and year.  --> 

 There are several methods we can use to investigate how bicycle volume may have changed over the four year period. 
 
Firstly we can look at the average monthly cyclist volume (total cyclists / sensor count, by year and overall). However, as there is large variation in the volume of cyclists recorded across the year, the median or 50th percentile for sensor volume may provide a better sense of usual monthly cyclist volume. The total number of cyclists observed in a particular year should also be understood relative to the number of sensors that were present in that year (monthly sensor counts). 

Whether you look at the mean or median number of cyclists, we see that there has been an overall decline in cycling volume in 2020 and 2021. 

                                                 
| Year                     |   Monthly sensor counts | Number of cyclists | Average monthly cyclists | Median monthly cyclists |
|--------------------------|------------------------:|-------------------:|-------------------------:|------------------------:|
| 2018                     |                     882 |         11,350,902 |                 12,869.5 |                10,365 |  
| 2019                     |                     963 |         13,064,949 |                 13,566.9 |                10,338 |  
| 2020                     |                    1,016|         11,803,715 |                 11,617.8 |                 9,267.5 | 
| 2021 (excl. Nov, Dec)    |                     908 |          9,625,145 |                 10,600.4 |                 8,933.5 |
| **Overall**              |                **3769** |     **45,844,711** |             **12,163.6** |            **9,813** |         

<br>

To analyse how public health measures may have affected cycling behaviour, we've aggregated the data further into weekly intervals. These weeks have then been aligned to the level of restrictions in place at that time. 

While January 2018 - Februrary 2020 had no restrictions on mobility in place, the remainder of 2020 and 2021 saw a mix of partial and full restrictions. Here we've differentiated partial and full restrictions by the lockdown level, with full restrictions corresponding to level 3 and level 4, and partial restrictions to level 1 and level 2.[^2]

Looking at the average number of weekly cyclists measured,  there is a significant decrease during partial and full restrictions in comparision to periods of no restrictions. 


| Restriction Level | Average weekly cyclists|
|-------------------|------------------------|
|              None |                 3161.4 |
|           Partial |                 2360.5 |
|              Full |                 2386.5 |
|        **Overall**|              **2797.5**|

This decline can also be seen when the distribution of sensor data is plotted. While periods with no restrictions had a weekly median of 2560 cyclists, the median of partial and full restrictions are lower and approximately similar, at 2002 and 2025 respectively.


##### Weekly bicycle volume by restriction level
*Hover to view median, upper and lower quartile ranges, as well as outlying data.*

<iframe src="/data_stories/visuals/bicycle_flows/Restriction_volume.html" allowfullscreen class="video-wrap full-width" height="600px" style="border:none;"></iframe>


#### Speed
<br>
If we compare the monthly average speeds across each of the years, we can see a small but significant reduction in average cycling speeds in 2020, and to a lesser extent for 2021.

While the data does not contain any qualitative data on cyclist demographics, both partial and full retrictions included directives to work from home if possible. The likely decrease in cyclists commuting to work could go some way in explaining the drop in speed across the network during these periods. 

| Restriction level | Average speed |
|-------------------|---------------|
|              None |          21.2 |
|           Partial |          20.4 |
|              Full |          19.5 |
|       **Overall** |      **20.7** |

<br>
###### Bicycle speed (km/hr) by month
*Hover over each data point to compare the average bicycle speed by month.*

<iframe src="/data_stories/visuals/bicycle_flows/speed_chart.html" allowfullscreen class="video-wrap full-width" height="500px" style="border:none;"></iframe>

#### Direction
<br>
With the cycling commute interrupted by pandemic restrictions, were we cycling in different directions?  

While across the period there does appear to be a reduction in North/South journeys, and an increase in North West/South travel, the extent to which we can interpret this trend is limited, as:

- The directions measured are dependent on where the sensors are located. 
- The 2021 data does not include November and December.
- Introduction of sensors in new locations could also affect shifts in directional volume.

<br>
###### Cycling direction by year
*Toggle between the years using the buttons below the polar charts. The radial scale represents the total number of cyclists in millions.*
<br>

{% include post-components/gallery.html
	columns = 1
	full_width = false
	images = "/data_stories/visuals/bicycle_flows/Sensor_Direction_2018.svg,/data_stories/visuals/bicycle_flows/Sensor_Direction_2019.svg,/data_stories/visuals/bicycle_flows/Sensor_Direction_2020.svg,/data_stories/visuals/bicycle_flows/Sensor_Direction_2021.svg"
%}

<br>
#### Location
<br>
Public health measures in 2020 and 2021 also affected where we cycled. 

The chart below compares the 2018-19 and 2020-21 bicycle traffic for each sensor site. As November and December are yet to be added to the 2021 data, we've reduced each year to a period from January to October to enable a fair comparison. 

Very few sensor sites maintained the same amount of bicycle traffic across the two periods, with the largest shifts taking place at Darebin Creek Trail and the Wellington Street sites.

<br>

###### Traffic comparison by sensor (2018/19 and 2020/21)
*The closer the colour split is to the central line, the more constant the bicycle volume across the period. We've removed any sensors that were not in place for the majority of the 4 year period.*
<iframe src="/data_stories/visuals/bicycle_flows/Sensor_by_split_years_comparison.html" allowfullscreen class="video-wrap full-width" height="500px" style="border:none;"></iframe>

<br>

When distance from the CBD is factored into sensor volume, we can see that sites further from the CBD experienced the highest growth in bicycle traffic in the 2020-21 period. Inversely, the closer to the city centre that a sensor was, the more likely that a decrease in bicycle traffic was observed.[^3]
 
<br>

###### Traffic change by sensor distance from CBD (2018/19 and 2020/21)
*The chart below uses a logarithmic scale for distance to CBD - the further from the city, the more pronounced the change in traffic volume. Hover to view the two year period, cyclist percentage of sensor, site and distance from CBD.*
<iframe src="/data_stories/visuals/bicycle_flows/Cyclist_percentage_distance_cbd.html" allowfullscreen class="video-wrap full-width" height="500px" style="border:none;"></iframe>

#### Conclusion
<br>

While Melbourne's bicycle traffic remained relatively constant during the public health measures in 2020/2021, the shifts in some of the metrics point to how our cycling habits may have changed during this period. 

- During periods of partial and full restrictions, there was less bicycle traffic than usual.
- On average, we cycled slightly more slowly.
- We cycled in different areas, with outer city sensor locations experiencing the highest increase in traffic.
 
<br>

---

##### Tools
<br>

*This analysis was produced using the open source software: [Python](https://www.python.org/) and [Jupyter notebook](https://jupyter.org/), and other Python modules including [Pandas](https://pandas.pydata.org/) and [Plotly](https://plotly.com/) available through the [Anaconda](https://www.anaconda.com/products/individual) Python distribution; [Git](https://git-scm.com/) version control; [Jekyll](https://jekyllrb.com/) for website development; [Github Pages](https://pages.github.com/) for hosting. If you're interested in the code used to create visualisations, you can follow along on the [blog](https://caropattle.github.io/data_stories/blog/) and find the project code repository [here](https://github.com/CaroPattle/data_stories/tree/main/bicycle_flows).*



---
[^1]: Fenwick St, Heidelberg Rd No.1 & No.2 were most likely installed post 2019, as there is only sensor data from 2020/21 for these sites.
[^2]: The timeline and restriction levels were cross-checked with several sources: [lockdownstats](https://lockdownstats.melbourne/timeline/), [the timeline of every Victorian lockdown](https://bigaustraliabucketlist.com/victoria-lockdowns-dates-restrictions/) and [Melbourne Lockdown Dates](https://www.platinumaccounting.com.au/melbourne-lockdown-dates/)
[^3]: Distance from the CBD, as represented by the intersection of Bourke and Elizabeth St and measured using Euclidean distance in metres ("as the crow flies").







