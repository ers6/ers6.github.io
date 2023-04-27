---
name: Testing IA Scanning Center Dashboard
tools: [Python, HTML, vega-lite]
image: assets/pngs/cars.png
description: This is a "showcase" project that uses vega-lite for interactive viz!
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---

# What's in the internet archive? 

<vegachart schema-url="{{ site.baseurl }}/assets/json/ia-contents-bar-chart.json" style="width: 100%"></vegachart> 

# When and Where were Books in the Internet Archive Scanned?

The number of books in the Internet Archive had increased steadily over time, rising from just 20,000 in 2005 to 37 million in 2023. 

<vegachart schema-url="{{ site.baseurl }}/assets/json/total_book_scans.json" style="width: 100%"></vegachart> 

# Example Draft Dashboard of IA Scanning Center Data

<vegachart schema-url="{{ site.baseurl }}/assets/json/geodash.json" style="width: 100%"></vegachart> 



## Search The Data & Methods

Below is where we can put some links to both the data and the analysis code as buttons:

```
<div class="left">
{% include elements/button.html link="https://github.com/vega/vega/blob/main/docs/data/cars.json" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://blog.4dcu.be/programming/2021/05/03/Interactive-Visualizations.html" text="The Analysis" %}
</div>
```

<!-- these are written in a combo of html and liquid --> 

{% include elements/button.html link="https://github.com/vega/vega/blob/main/docs/data/cars.json" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/jnaiman/online_cv_public/blob/main/python_notebooks/test_generate_plots.ipynb" text="The Analysis" %}
</div>

