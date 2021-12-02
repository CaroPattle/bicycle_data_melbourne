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

The following visualisations use [open data](https://discover.data.vic.gov.au/dataset/bicycle-volume-and-speed) to investigate Melbourne’s bicycle traffic across the last four years. 

Melbourne bicycle volume and speed are recorded by sensors at 42 off-road and 4 on-road counter sites. Most sites have two sensors embedded in the pavement to measure bi-directional bicycle flows.

The dataset includes information such as the volume of cyclists crossing the sensor, their speed, the gap between cyclists, as well as measurements on the wheelbase and axles which indicate the type of bike being ridden.

The map below shows the **location**, and **monthly average speed** and **number of cyclists** from Jan 2018 - Oct 2021.

*Hover over a specific site in the map below to view the monthly total of cyclists and their average speed.*

<!-- ![](../images/Sensor_Site_Map.png) -->

<iframe src="/data_stories/visuals/bicycle_flows/Sensor_Map.html" class="video-wrap full-width" height="600px"  style="border:none;"></iframe>

Across the four years there were **46 million bicycles** registered by the network of sensors across Melbourne. For convenience we'll refer to each bicycle registered by a sensor as a cyclist. 

| Year                     | Number of cyclists | Average speed (km/h) |
|--------------------------|-------------------:|---------------------:|
| 2018                     |         11,350,902 |                 21.2 |
| 2019                     |         13,064,949 |                 21.3 |
| 2020                     |         11,803,715 |                 19.8 |
| 2021 (excludes Nov, Dec) |          9,625,145 |                 20.6 |
| **Overall**              |     **45,844,711** |             **20.7** |

<br>

###### Bicycle volume by sensor
<br>
Let’s breakdown the total volume of cyclists measured by each sensor across the four years.

-There's a broad range of **bicycle traffic volume** recorded by sensors across the network from **26 thousand to 2.8 million cyclists**.

-Fenwick St, Heidelberg Rd No.1 & No.2 were most likely installed post 2019, as there is only sensor data from 2020/21 for these sites.


*Scroll to see the complete list, hover to view percentage*

<iframe src="/data_stories/visuals/bicycle_flows/Sensor_by_volume.html" class="video-wrap full-width" height="400px"  style="border:none;"></iframe>
<br>

#### The pandemic

2020 and 2021 were extraordinary years.  From late 2019, Victoria was affected by [devastating bush fires](https://www.vic.gov.au/2019-20-eastern-victorian-bushfires) and a State of Disaster was declared on 2 January 2020.  Due to the smoke, health warnings were issued with Melbourne's [air quality](https://www.theguardian.com/australia-news/2020/jan/14/melbourne-choked-by-hazardous-smoke-as-bushfires-continue-to-burn-across-victoria) said to be the 'worst in the world' in mid-January. 

From March 2020 and through 2021, Melbourne enacted a broad range of [public health measures to curb the spread of Covid-19](https://www.dhhs.vic.gov.au/coronavirus-update-victoria-26-march-2020). These restrictions spanned density limitations in public spaces and the donning of masks outside the home, through to measures aimed at minimising population mobility.  

Let's see if the impact of these events are reflected in the bicycle traffic data. 

<br>
###### Monthly bicycle volume and speed by sensor
<br>
The visualisation below charts the monthly total of cyclists, and their average speed, for each sensor across the four year period.

-**October 2020/2021** saw cyclists travelling at **lower speeds** than in 2018/2019, with **lower bicycle volumes** on popular **inner city commuting routes**.

-**June**, **July** and **August** saw the **least bicycle traffic** across all of the years – fewer of us brave Melbourne winters on bikes.

*Each bubble in the chart represents a sensor. Move the slider to view monthly speed and volume.*

<iframe src="/data_stories/visuals/bicycle_flows/BubbleYears.html" allowfullscreen class="video-wrap full-width" height="600px" style="border:none;"></iframe>

<br>

###### Bicycle speed (km/hr) by month
<br>
Let's compare the monthly average speeds across each of the years. 

-There was a small but significant **reduction** in **average cycling speeds** in **2020**, and to a lesser extent for **2021**

*Hover over each data point to compare the average bicycle speed by month.*

<iframe src="/data_stories/visuals/bicycle_flows/speed_chart.html" allowfullscreen class="video-wrap full-width" height="500px" style="border:none;"></iframe>


###### Cycling direction by year
<br>

With the cycling commute interrupted by pandemic restrictions, were we cycling in different directions?  

While across the period there does appear to be a **reduction in North/South** journeys, and an **increase in North West/South** travel, the extent to which we can interpret this trend is limited, as:

- The directions measured are dependent on where the sensors are located. 
- The 2021 data does not include November and December.
- Introduction of sensors in new locations could also affect shifts in directional volume.


*Toggle between the years using the buttons below the polar charts*

{% include post-components/gallery.html
	columns = 1
	full_width = false
	images = "/data_stories/visuals/bicycle_flows/Sensor_Direction_2018.svg,/data_stories/visuals/bicycle_flows/Sensor_Direction_2019.svg,/data_stories/visuals/bicycle_flows/Sensor_Direction_2020.svg,/data_stories/visuals/bicycle_flows/Sensor_Direction_2021.svg"
%}



###### Comparison of bicycle traffic by sensor
<br>
Has the impact on Melbourne's mobility impacted where we cycle?

The chart below compares the 2018-19 and 2020-21 bicycle traffic for each sensor site. As November and December are yet to be added to the 2021 data, we've reduced each year to a period from January to October to enable a fair comparison. 

-The sensors that saw the **greatest increases** in bicycle volume in 2020-21 were **Darebin Creek Trail**, **Ann Trail No.3**, **Christmas St**, **Box Hill\\Ringwood Trail**, and **Federation Trail**.

-The sensors that saw the **greatest decreases** in bicycle volume in 2020-21 were **Napier St Path**, **Brighton Rd**, **Flemington Rd**, **Royal Pde**, and **Wellington St**.

*The closer the colour split is to the central line, the more constant the bicycle volume across the period. We've removed any sensors that were not in place for the majority of the 4 year period.*

<iframe src="/data_stories/visuals/bicycle_flows/Sensor_by_split_years_comparison.html" allowfullscreen class="video-wrap full-width" height="500px" style="border:none;"></iframe>


#### Trends
To what degree can we say that public health measures influenced Melbourne bicycle traffic?

For the purposes of this analysis, we've aligned weeks of the year to their respective restriction levels, with 2018-19 having no restrictions, and 2020/21 a mix of partial and full restrictions.[^1] 

<br>

###### Correlation Matrix
<br>
The correlation matrix below represents the direction and strength of associations between variables. The first two variables, total cyclists and average speed, are outcomes of interest, while the other variables are exposures which may, or may not, influence these outcomes. 

-A weak association between **'No restrictions'** and **average speed** is in line with the **speed decrease in 2020/21** as seen in our other analyses.

-While there was a **weak negative association** between **cycling speed** and periods of **high restrictions**, this was not seen during partial restrictions where increased mobility such as travel to work was less restricted.

-**Distance from the CBD** had a weak negative correlation with **speed**, but more so with **total number of cyclists**[^2]. The further from the centre of Melbourne sensors were placed, the fewer, and on average slightly slower, cyclists were recorded.

*Association strength ranges from -1 to +1, with zero indicating no correlation. Dark grey indicates a strong negative assocation, while dark blue indicates a strong positive association*

<iframe src="/data_stories/visuals/bicycle_flows/Correlation_Matrix.png" class="video-wrap full-width" height="600px"  style="border:none;"></iframe>


---

[^1]: Full and partial restrictions are respectively aligned to Stage 4/Stage 3 and Stage 2/Stage 1 public health measures. The absence of restrictions (2018-19) is inversely collinear with partial and full restrictions (2020-21).  If we were to model the relationship between restrictions and our outcomes of interest (Total cyclists and Average speed), we would use the indicator variables for partial and full restrictions and omit the variable for no restrictions, since this is effectively implied as the case when both partial and full restrictions are false.
[^2]: Distance from the CBD, as represented by the intersection of Bourke and Elizabeth St and measured using Euclidean distance in metres ("as the crow flies").







