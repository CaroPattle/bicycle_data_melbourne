# Melbourne Bicycle Volume & Speed
## Let's get the data!

16 November 2021

Welcome to the inaugural blog post!

In this blog we'll cover how we imported the dataset into a python coding environment, and readied the dataframe for analysis and visualisation. 

---

#### The dataset

Before starting, we've downloaded the bicycle volume and speed data located on the DataVic site [here](https://discover.data.vic.gov.au/dataset/bicycle-volume-and-speed)

The data shows cycling flows in both directions recorded at 42 off-road counter sites and 4 on-road counter sites in Melbourne.

The dataset is delivered in a large number of CSV files, with each file containing several days worth of data from one seonsor location. There's also an excel file called 'VicRoads_Bike_Site_Number_Listing' which indexes the location of each of the sensors. 

While the files could be programmatically unzipped with code, we unzipped them all using 7-zip in one big batch. Easy!

---

### The code

We'll start off by importing all the python libraries that we'll need in the one spot: 

```python:
import pandas as pd
import numpy as np
import os
from collections import Counter
from tqdm.notebook import tqdm
import plotly.express as px
import geopandas as gpd
import plotly.graph_objects as go
```

Then, let's create a couple of variables for the operating system file paths to access the CSVs downloaded from DataVic. This will save time later on!

```python:
rootdir = '../../data/DPC/bicycle_flows/'
visuals = '../docs/visuals/bicycle_flows/'
```

#### Data validation

There's a lot of CSV files, so lets first make sure that each CSV has the same variables or columns. Once this is confirmed, we'll be able to combine all of the individual files into a dataframe.

The code below iterates over each of the CSVs and tallies the number of unique column combinations. Ideally, the result will be a single combination of columns, so we'll be able to append each to a new dataframe. Let's see!

We'll also limit our data to the last 5 years, from 2017 to 2021

```python:
data_years = [2017,2018,2019,2020,2021]
folder_prefix = 'Bicycle_Volume_Speed_'

for year in data_years:
    tally = pd.DataFrame(columns=["count","len"])
    counter = 0
    for subdir, dirs, files in tqdm(os.walk(rootdir)):
        for file in files:
            if ('.csv' in file) and ('.zip' not in file):
            # read in CSV, if it contains records (which at least one doesn't!)
                file_path = os.path.join(subdir,file) 
                if os.path.getsize(file_path) > 0:
                    df = pd.read_csv(os.path.join(subdir,file))
                # store list of columns in variable df_columns as a string
                    df_columns = f"{df.columns.to_list()}"
                    # if CSV columns string is in the tally index, increment this
                    if df_columns in tally.index:
                        tally[tally.index==df_columns] += 1
                        # otherwise add CSV columns string to the tally index
                    else:
                        tally.loc[df_columns] = 1
                        # increment a counter; athough theoretically this should only sum to the sum of tallies!
                        counter+=1

print(counter)
```









![](/images/demo/work-01.jpg)

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

[^1]: Beautiful modern, minimal theme design.
[^2]: Powerful features to show off your work.
[^3]: Maintained and supported by the theme developer.

You can throw in some horizontal rules too:

---

#### Image galleries

Here's a really neat custom feature we added – galleries:

{% include post-components/gallery.html
	columns = 2
	full_width = true
	images = "/images/demo/work-02.jpg,/images/demo/work-03.jpg,/images/demo/work-04.jpg,/images/demo/work-05.jpg,
	"
%}

Inspired by the Galleries feature from WordPress, we've made it easy to create grid layouts for your images. Just use a simple Liquid snippet in your post to create a masonry grid image layout:

{% raw %}
```liquid
{% include post-components/gallery.html
	columns = 2
	full_width = true
	images = "/images/demo/work-02.jpg,/images/demo/work-03.jpg,/images/demo/work-04.jpg,/images/demo/work-05.jpg,
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
	full_width = true
	images = "/images/demo/work-06.jpg,/images/demo/work-07.jpg,/images/demo/work-08.jpg
	"
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