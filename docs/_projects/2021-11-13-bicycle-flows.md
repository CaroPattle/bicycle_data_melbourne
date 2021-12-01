---
title: Melbourne Bicycle Traffic
subtitle: How has the Covid-19 pandemic changed our cycling habits? Let’s see.

date: 2021-11-13 00:00:00
description: Analysis of Melbourne bicycle traffic using open data

featured_image: '../Sensor_Site_Map.png'
accent_color: '#4C60E6'
gallery_images:
  - '../Sensor_Direction_2018.png'
  - '../Sensor_Direction_2019.png'
  - '../Sensor_Direction_2020.png'
  - '../Sensor_Direction_2021.png'
---

#### The data

The following visualisations use [open data](https://discover.data.vic.gov.au/dataset/bicycle-volume-and-speed) to investigate Melbourne’s bicycle traffic across the last four years. 

Melbourne bicycle volume and speed are recorded by sensors at 42 off-road and 4 on-road counter sites. Most sites have two sensors embedded in the pavement to measure bi-directional bicycle flows.

The dataset includes information such as the volume of cyclists crossing the sensor, their speed, the gap between cyclists, as well as measurements on the wheelbase and axles which indicate the type of bike being ridden.

The map below shows the location, and monthly average speed and number of cyclists from Jan 2018 - Oct 2021.

*Hover over a specific site in the map below to view the monthly total of cyclists and their average speed.*

<!-- ![](../images/Sensor_Site_Map.png) -->

<iframe src="/data_stories/visuals/bicycle_flows/Sensor_Map.html" class="video-wrap full-width" height="600px"  style="border:none;"></iframe>

Across the four years there were 46 million bicycles registered by the network of sensors across Melbourne. For convenience we'll refer to each bicycle registered by a sensor as a cyclist. 

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

- **There's a broad range of traffic volume, from 26 thousand to 2.8 million cyclists**
- **Fenwick St, Heidelberg Rd No.1 & No.2 were most likely installed post 2019, as there is only sensor data from 2020/21 for these sites**


*Scroll to see the complete list, hover to view percentage*

<iframe src="/data_stories/visuals/bicycle_flows/Sensor_by_volume.html" class="video-wrap full-width" height="400px"  style="border:none;"></iframe>
<br>

#### The pandemic

2020 and 2021 were extraordinary years.  From late 2019, Victoria was effected by [devastating bush fires](https://www.vic.gov.au/2019-20-eastern-victorian-bushfires) and a State of Disaster was declared on 2 January 2020.  Due to the smoke, health warnings were issued with Melbourne's [air quality](https://www.theguardian.com/australia-news/2020/jan/14/melbourne-choked-by-hazardous-smoke-as-bushfires-continue-to-burn-across-victoria) said to be the 'worst in the world' in mid-January. From March 2020 and through 2021, Melbourne enacted a broad range of [public health measures to curb the spread of Covid-19](https://www.dhhs.vic.gov.au/coronavirus-update-victoria-26-march-2020). These restrictions spanned density limitations in public spaces and the donning of masks outside the home, through to measures aimed at minimising population mobility.  Due to these unprecedented disruptions, one would expect some impact on normal cycling behaviours.

<br>
###### Monthly bicycle volume and speed by sensor
<br>
The visualisation below charts the monthly total of cyclists, and their average speed, for each sensor across the four year period.

* **October 2020/2021 saw cyclists travelling at lower speeds than in 2018/2019, with reduced ridership on popular inner city commuting routes**
* **June, July and August saw the least bicycle traffic across all of the years – fewer of us brave Melbourne winters on bikes**

*Each bubble in the chart represents a sensor. Move the slider to view monthly speed and volume.*

<iframe src="/data_stories/visuals/bicycle_flows/BubbleYears.html" allowfullscreen class="video-wrap full-width" height="600px" style="border:none;"></iframe>

<br>

###### Bicycle speed (km/hr) by month
<br>
Let's compare the monthly average speeds across each of the years. 

* **There was a small but significant reduction in average cycling speeds in 2020, and to a lesser extent for 2021**

*Hover over each data point to compare the average bicycle speed by month.*

<iframe src="/data_stories/visuals/bicycle_flows/speed_chart.html" allowfullscreen class="video-wrap full-width" height="500px" style="border:none;"></iframe>


###### Cycling direction by year
<br>

With the cycling commute interrupted by pandemic restrictions, were we cycling in different directions?  While some interesting patterns are observable, with reduced North-South volume, and some increases in North west-South east trajectories in 2020, there are important caveats that limit the degree to which we can generalise these patterns to overall ridership:

- The directions measured depend on the locations where sensors have been placed
- The 2021 data does not include November or December, hence total volume is lower than for other years
- Introduction of sensors in new locations could be one source of apparent shift in directional volume, rather than general behavioural change 


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

* **The sensors that saw the greatest increases in bicycle volume in 2020-21 were Darebin Creek Trail, Ann Trail No.3, Christmas St, Box Hill\\Ringwood Trail, Federation Trail**
* **The sensors that saw the greatest decreases in bicycle volume in 2020-21 were Napier St Path, Brighton Rd, Flemington Rd, Royal Pde, Wellington St**

*The closer the colour split is to the central line, the more constant the bicycle volume across the period. Several sensors were only added post 2019.*

<iframe src="/data_stories/visuals/bicycle_flows/Sensor_by_split_years_comparison.html" allowfullscreen class="video-wrap full-width" height="500px" style="border:none;"></iframe>

<br>



#### Trends
<br>

The chart below is a correlation matrix which represents the direction and strength of associations between variables.  Weeks of the year were aligned with their restriction levels, with 2018-19 having no restrictions, and 2020/21 a mix of partial- and full restrictions.  In the correlation matrix, the first two listed variables of 'Total cyclists' and 'Average speed' are outcomes of interest, while levels of restrictions are exposures which we might hypothesise could bear some influence on these outcomes.

As observed earlier, the 2018-19 period prior to Covid19 related restrictions was weakly associated with increased average cycling speed.  Partial restrictions were not correlated with cycling speed, while a weak negative association with cycling speed was observed for high restrictions.  Distance from the CBD, as represented by the intersection of Bourke and Elizabeth St and measured using Euclidean distance in metres ("as the crow flies"), also had a weak negative correlation with speed, but more so with total number of cyclists.  

The absence of restrictions (2018-19) is inversely collinear with partial- and full restrictions (2020-21).  If we were to model the relationship between restrictions and our outcomes of interest, we would use the indicator variables for partial and full restrictions and omit the variable for no restrictions, since this is effectively implied as the case when both partial and full restrictions are false.

<iframe src="/data_stories/visuals/bicycle_flows/Correlation_Matrix.png" class="video-wrap full-width" height="450px"  style="border:none;"></iframe>

#### Conclusion
<br>










**Obviously,** we’ve styled up *all the basic* text formatting options [available in markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).

You can create lists:

* Simple bulleted lists
* Like this one
* Are cool

And:

1. Numbered lists
2. Like this other one
3. Are great too

You can also add blockquotes, which are shown at a larger width to help break up the layout and draw attention to key parts of your content:

> “Simple can be harder than complex: You have to work hard to get your thinking clean to make it simple. But it’s worth it in the end because once you get there, you can move mountains.”

The theme also supports markdown tables:

| Item                 | Author        | Supports tables? | Price |
|----------------------|---------------|------------------|-------|
| Duet Jekyll Theme    | Jekyll Themes | Yes              | $49   |
| Index Jekyll Theme   | Jekyll Themes | Yes              | $49   |
| Journal Jekyll Theme | Jekyll Themes | Yes              | $49   |

And footnotes[^1], which link to explanations[^2] at the bottom of the page[^3].

[^1]: 
[^2]: Powerful features to show off your work.
[^3]: Maintained and supported by the theme developer.

You can throw in some horizontal rules too:

---

#### Image galleries

Here's a really neat custom feature we added – galleries:

{% include post-components/gallery.html
	columns = 2
	full_width = true
	images = ""
%}

Inspired by the Galleries feature from WordPress, we've made it easy to create grid layouts for your images. Just use a simple Liquid snippet in your post to create a masonry grid image layout:

{% raw %}
```liquid
{% include post-components/gallery.html
	columns = 2
	full_width = true
	images = "/../Sensor_Site_Map.png,/../Sensor_Site_Map.png,/../Sensor_Site_Map.png,/../Sensor_Site_Map.png,
	"
%}
```
{% endraw %}

*See what we did there? Code and syntax highlighting is built-in too!*

Change the number inside the 'columns' setting to create different types of gallery for all kinds of purposes. You can even click on each image to seamlessly enlarge it on the page.


#### Image carousels

Here's another gallery with only one column, which creates a carousel slide-show instead.

A nice little feature: the carousel only advances when it is in view, so your visitors won't scroll down to find it half way through your images.

{% include post-components/gallery.html
	columns = 1
	full_width = false
	images = "/data_stories/visuals/bicycle_flows/Sensor_Direction_2018.svg,/data_stories/visuals/bicycle_flows/Sensor_Direction_2019.svg,/data_stories/visuals/bicycle_flows/Sensor_Direction_2020.svg,/data_stories/visuals/bicycle_flows/Sensor_Direction_2021.svg"
%}

#### What about videos?

Videos are an awesome way to show off your work in a more engaging and personal way, and we’ve made sure they work great on our themes. Just paste an embed code from YouTube or Vimeo, and the theme makes sure it displays perfectly:

{% include post-components/video.html
	url = "https://player.vimeo.com/video/270725085?color=6c6e95&title=0&byline=0"
	full_width = true
%}

### Pretty cool, huh?

We've packed this theme with powerful features to show off your work.
Why not put them to use on your new website?

<a href="https://jekyllthemes.io/theme/made-portfolio-jekyll-theme" class="button--fill">Get This Theme</a>