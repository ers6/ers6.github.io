---
name: Altair-generated Vega Lite Plots of Bigfoot Dataset
tools: [Python, HTML, vega-lite]
image: /assets/pngs/bigfoot.png
description: Homework 10 visualizes the bigfoot sightings dataset to explore the interactive visualization capabilities of Altair and Vega Lite
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Map of All Bigfoot Sightings in the Dataset with Mouseover 

<vegachart schema-url="{{ site.baseurl }}/assets/json/mouse_over_map.json" style="width: 100%"></vegachart>

## Write-Up 

This map visualizes every sighting of bigfoot in the dataset plotted by latitude and longitude. You can mouse-over each sighting to reveal the title of the sighting as entered in the dataset. I encoded the latitude and longitude data using altair's latitude and longitude encoding type and made their data-type quantitative. I did not transform the data in anyway nor did I filter it. However, I did add an interactive element to the visualization. I think this map could function as the driver of a dashboard where each point could include an href linking out to another page of the website on the sighting. In this way, this visualization could work as a landing page for a bigfoot sighting database. 


# Dashboard of All Bigfoot Sightings in Latitude and Longitude Ranges Over Time

<vegachart schema-url="{{ site.baseurl }}/assets/json/scatter_driver.json" style="width: 100%"></vegachart>

## Write-Up 

This dashboard links the latitude and longitude range of bigfoot sightings on a scatter plot to a bar chart counting the number of bigfoot sightings within the latitude and longitude range per year. I encoded the latitude and longitude as x and y encoding types and quantitative data types. This is because I wanted to use a scatter plot. Moreover, I colored point on the scatter plot based on the season in which the sighting occurred. I encoded the the year data in the second chart as temporal. The count of records per year in the y field of the second chart is quantitative by default. In this plot, I used altair's time unit transformations to extract just the year from the date information in the dataset. This visualization is most similar to those I created in starboard for homework 9. For Homework 9, I created 2 visualizations: one visualized the number of bigfoot sightings per state and another visualized bigfoot sightings over time. This visualization enables a user to see the temporal patterns of bigfoot sightings in a latitude and longitude range of their choosing. 


# Search The Data & Methods

Both plots 1 and 2 were created using the same dataset within the same jupyter notebook. View both below. 


<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/main/data/bfro_reports_fall2022.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://blog.4dcu.be/programming/2021/05/03/Interactive-Visualizations.html" text="The Analysis" %}
</div>

