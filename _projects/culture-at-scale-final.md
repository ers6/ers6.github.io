---
name: Scanning at Scale
tools: [Python, HTML, vega-lite]
image: assets/pngs/cars.png
description: This is a "showcase" project that uses vega-lite for interactive viz!
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Map 

<vegachart schema-url="{{ site.baseurl }}/assets/json/interactive_map.json" style="width: 100%"></vegachart>


# Datum Data Co. Ltd. 

<vegachart schema-url="{{ site.baseurl }}/assets/json/datum_data_ship_viz.json" style="width: 100%"></vegachart>

# Internet Archive China

<vegachart schema-url="{{ site.baseurl }}/assets/json/hongkong_ships_viz.json" style="width: 100%"></vegachart>

# Innodata Knowledge Services

<vegachart schema-url="{{ site.baseurl }}/assets/json/cebu_ship_viz.json" style="width: 100%"></vegachart>


<!-- these are written in a combo of html and liquid --> 


{% include elements/button.html link="https://github.com/vega/vega/blob/main/docs/data/cars.json" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/jnaiman/online_cv_public/blob/main/python_notebooks/test_generate_plots.ipynb" text="The Analysis" %}
</div>
