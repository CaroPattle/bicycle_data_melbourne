---
title: Building Permit Activity
subtitle: How has the Covid-19 pandemic affected the Victorian construction industry?

date: 2022-01-18 00:00:00
description: Analysis of Victorian building permit activity using open data

featured_image: '../permit_map_2021.jpg'
accent_color: '#4C60E6'
gallery_images:
  - '../../visuals/bicycle_flows/Map snip-01.svg'
---



Over the last 2 years the Victorian construction industry has experienced both the [economic volatility](https://www.abs.gov.au/statistics/economy/national-accounts/australian-national-accounts-national-income-expenditure-and-product/sep-2021) caused by the Covid19 pandemic as well as the fiscal measures aimed at mitigating its effects.

In the face of the first recession in 30 years, the Federal Government unveiled the [HomeBuilder](https://www.sro.vic.gov.au/homebuilder-grant-guidelines)  initative in June 2020, targeting the construction industry as one of the national economy's key players. The scheme aimed to support confidence in the residential construction sector by providing eligible owner-occupiers with a grant to build a new home, substantially renovate an existing home or buy an off-the-plan home/new home.

In Victoria alone, the HomeBuilder initiative recieved just over [39,000](https://treasury.gov.au/coronavirus/homebuilder) applicants. However, to what degree can we say that the state's construction industry not only weathered but thrived during the pandemic? This analysis will use [open data building permit activity](https://discover.data.vic.gov.au/dataset/building-permit-activity-data-2020) as one measure of the sector's resilience. Comprised of over 40 variables, the annual building permit datasets provide a range of insights into how many Victorians are deciding to build, where and how they're building, as well as any shifts in these behaviours. 


#### Volume

As a basic measure, let's first investigate the volume of building permits issued. 

Between January 2019 to November 2021, over 330,000 building permits were issued in Victoria.

Breaking this down annually, we can observe that building permit volume actually grew across the period, with both 2020 and 2021 seeing an increase in the total number of building permits issued. This trend will become yet more apparent as the December 2021 data is added to the dataset.

<br>

###### Building permit volume by year 

*Hover to view annual permit volume totals*

<iframe src="/data_stories/visuals/building_permits/Permit_Volume_Bar.html" class="video-wrap full-width" height="600px"  style="border:none;"></iframe>

Viewing the permit volume by month we can see the likely impact of the HomeBuilder scheme. While the building permit volume fluctuated from month to month, the highest spike of the period occured in March 2021, with 12,400 permits issued.  This was immediately prior to the conclusion of the initiative in April of that year.

<br>

###### Building permit volume by month
*Hover to view the permit volume by month*


<iframe src="/data_stories/visuals/building_permits/Permit_Volume_Line_Monthly.html" class="video-wrap full-width" height="600px"  style="border:none;"></iframe>



#### Location, location, location

While there were overall annual increases in permit volume between 2019 and 2021, this growth was not distributed uniformly across Victoria. Between 2020 and 2019, fewer than half of Victorian suburbs experienced permit volume growth, while between 2021 and 2020 this had reduced to 39% of suburbs.

Across the entire period, the ten suburbs below saw the highest volume of Victorians choosing to build.


| Suburb      |   2019 |   2020 |   2021 |   3-year Total |
|:------------|-------:|-------:|-------:|---------------:|
| Tarneit     |   1239 |   2378 |   2153 |           5770 |
| Truganina   |   1176 |   1712 |   2045 |           4933 |
| Melbourne   |   1907 |   1349 |   1343 |           4599 |
| Clyde North |   1162 |   1132 |   1764 |           4058 |
| Wollert     |   1238 |   1437 |   1019 |           3694 |
| Werribee    |   1366 |   1125 |   1069 |           3560 |
| Craigieburn |   1070 |   1087 |    932 |           3089 |
| Mickleham   |    977 |   1151 |    958 |           3086 |
| Clyde       |    944 |    896 |    681 |           2521 |
| Officer     |    727 |    641 |    832 |           2200 |


To view the relative locations of these suburbs, we can link the building permit data with digital boundaries for suburbs from the ABS 2021 release of the [Australian Statistical Geography Standard](https://www.abs.gov.au/statistics/standards/australian-statistical-geography-standard-asgs-edition-3/jul2021-jun2026/access-and-downloads/digital-boundary-files).  This allows us to view the distribution of permit volume within an interactive map.[^2]

Clusters of surburbs experiencing higher volumes of building activity can be identified on the urban fringe of Greater Melbourne. To the west, the neighbouring suburbs of Tarneit and Truganina, and to the East, the outer suburbs of Clyde North, Officer and Berwick, all experienced high demand for building permits. 

<br>

###### Victorian building permit volume by suburb

*Hover to view specific suburb volume*

<iframe src="/data_stories/visuals/building_permits/Choropleth Volume Map.html" class="video-wrap full-width" height="600px"  style="border:none;"></iframe>



 

<br>

#### Activity

The building permit dataset also gives us insight into the type of building activities for which planning permits have been issued.

The chart  below displays specific construction activities as a percentage of each suburb's total building permits.

With the exception of Melbourne, the bulk of activity in top ranking suburbs is related to new builds. This finding is not altogether suprising given the differences in urban density when comparing the city centre with suburbs located on the urban fringe. 

<iframe src="/data_stories/visuals/building_permits/Parallel coordinates plot.html" class="video-wrap full-width" height="600px"  style="border:none;"></iframe>

<br>


#### Building Use


While demand for building permits grew between 2019 and 2021, there were several shifts in the types of buildings that were being constructed.

While permits relating to commercial and public buildings decreased, both industrial and domestic builds experienced sustained growth overall across the three year period. Perhaps surprisingly, hospital and healthcare building permits also decreased across the period.

These shifts are likely explained in part by the focus of the HomeBuilder fund, which targeted home owners looking to spend on domestic construction. They also perhaps point to a recalibration of priorities in a pandemic economy, with a new emphasis on working from home and less of an imperative to spend on commercial and public buildings. 



| Building Use         |   2019 |   2020 |   2021 |
|:---------------------|-------:|-------:|-------:|
| Commercial           |   7031 |   6917 |   6894 |
| Domestic             |  83928 |  96368 | 102476 |
| Hospital/Healthcare  |    522 |    407 |    423 |
| Industrial           |   1268 |   1595 |   1623 |
| Public Buildings     |   4107 |   4066 |   3611 |
| Residential          |    811 |    657 |    820 |
| Retail               |   4321 |   3420 |   3721 |
| TOTAL                | 101988 | 113430 | 119568 |

<br>



#### Cost

Although we can see that Victorians were still keen to spend on construction during 2020 and 2021, was this enthusiasm matched with an increase in budget?

Charting the median estimated building cost by month, we can see that, despite some fluctuations, the estimated cost listed per permit increased between 2019 and 2021.[^1]

However, while 2020 spending was relatively steady, its highest point in September was  still below the corresponding peak in 2019. This observation may reflect the income-capped eligibility requirements of HomeBuilder, with individual applicants required to earn below $125k and couples below $200k per annum. 

Perhaps concerningly, the largest and most sustained decrease in median of construction budgets was seen in late 2021, which coincided with the arrival in Australia of the Delta Covid19 variant.

<br>

###### Median building cost by month

*Hover over each data point to compare the average estimated build cost by month*

<iframe src="/data_stories/visuals/building_permits/Median_Monthly_Cost_By_Year.html" class="video-wrap full-width" height="600px"  style="border:none;"></iframe>



#### Environment

Victorians are increasingly investing portions of their construction budget on features that harness natural resources. 

The barchart below shows a steady increase in the percentage of building permits which include plans for solar hot water systems and/or rainwater tanks. This increase indicates a growing market for climate-conscious construction.

<br>

###### Solar hot water and rainwater tank inclusion by year
*Hover to view annual percentages*

<iframe src="/data_stories/visuals/building_permits/Eco_Features_Bar.html" class="video-wrap full-width" height="600px"  style="border:none;"></iframe>


#### Conclusion
<br>
The building permit dataset provides evidence that, despite global economic uncertainties, the Victorian construction industry experienced growth across the pandemic period.

Analysing several key variables, we can see that:

- There was growth in building permit volume.
- The median spend per planning permit increased.

While new builds dominated in the urban fringe suburbs which experienced high permit volume, this trend was reversed in inner Melbourne, where alterations comprised the bulk of permits.

However, there were several metrics which point to the effects of an economy operating in a pandemic. Firstly we saw a shift in the intended purposes of buildings, with a move away from commmercial and public buildings and an increase in domestic and industrial builds. Secondly, although the median construction budget increased annually, a steep decline was observable in late 2021, coinciding with the arrival of a new Covid19 variant and the conclusion of the HomeBuilder stimulus. 

And finally, Victorians are increasingly looking to include building features which harness their natural environment, with a growth in the uptake of both solar hot water and rainwater tanks .

 
<br>

---

##### Tools
<br>

*This analysis was produced using the open source software: [Python](https://www.python.org/) and [Jupyter notebook](https://jupyter.org/), and other Python modules including [Pandas](https://pandas.pydata.org/) and [Plotly](https://plotly.com/) available through the [Anaconda](https://www.anaconda.com/products/individual) Python distribution; [Git](https://git-scm.com/) version control; [Jekyll](https://jekyllrb.com/) for website development; [Github Pages](https://pages.github.com/) for hosting. If you're interested in the code used to create visualisations, you can follow along on the [blog](https://caropattle.github.io/data_stories/blog/) and find the project code repository [here](https://github.com/CaroPattle/data_stories/tree/main/bicycle_flows).*



---

[^1]: The building permit dataset records both the estimated cost and the reported cost of the build. For building permits issued on or after 1 July 2019, permit recipients are required to monitor and report on the final project spend. For the purposes of this analysis, we've used the cost estimated at the time of the permit issue.
[^2]: Linkage with the ABS ASGS Suburbs and Localities data requires a match on the suburb name, however some data cleaning was required to ensure the spelling and formatting of the suburb records (manually entered in the permits data) could find an exact match.  Common patterns were able to be accounted for, however due to some typographical errors or ambiguous names in the source data a small number of records (< 0.3%) were unable to be matched.







