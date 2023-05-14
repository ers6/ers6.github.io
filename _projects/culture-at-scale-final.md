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

# Scanning at Scale
In a former Christian Science church in San Francisco, petabytes of servers store thousands of cassettes, millions of books, and billions of web pages. This place where technophiles come to worship is known as the Internet Archive. Founded in 1996 by a dot com era billionaire, Brewster Kahle, the Internet Archive initially aimed to archive all of the world wide web. 27 years later in 2023, the Internet Archive is now the world’s largest free digital library boasting over 800 billion webpages, 37 million books and texts, 15 million audio recordings, 9.7 million videos, 4.6 million images, and 983 thousand software programs. As such, it is a crucial piece of scholarly infrastructure enabling the study of culture at scale.

Aside from the 800 billion webpages, the digitization of which can be automated via web crawlers, human workers digitize all other content of the internet archive. This project is concerned with the digitization process through which the second most common content type--books--were ingested into the archive. Internet Archive announced the launch of its book scanning program with a December 2004 blog post. According to the post, the program began as a partnership between Internet Archive and ten academic libraries across the world in an effort to digitize free, open access versions of books made available to the public via the web (Kaplan “Open Text Archives”). In the months that followed, Internet Archive set up scanning centers in partner-institution libraries. While Internet Archive celebrates some scanning workers and scanning centers on their blog, the process through which the books are scanned remains opaque. 

*[Scanning Labor in the Internet Archive](https://scanninglabor.github.io/IAScanningLabor/index.html)* is a DH project that seeks to remedy this gap. Through a data-enabled spatial, labor, and oral history, Scanning Labor sheds light on and reappraises the work of book scanning workers in the Internet Archive. Scanning Labor analyzed 2.5 million metadata records of books and texts that IA scanning workers digitized between 2004 and 2022. Each scanning record contains information about the date upon which the book was scanned and the name of the scanning center at which the scan was captured. While the 2.5 million records are a small subset of all the books and texts in the internet archive, analysis of them revealed that around 2011 Internet Archive shifted most of its book scanning operations from in-house scanning centers at academic libraries in the global north to shipping vast quantities of books overseas for digitization at business process outsourcing firms in the global South. The shift from academic library scanning operations is also associated with a sharp uptake in the number of total books scanned per month and the number of books scanned per worker per day. However, IA rarely mentions these outsourced scanning centers in public press releases, and when pressed about them, Internet Archive officials ceased communication with our team and engagement with the *Scanning Labor* project.

<vegachart schema-url="{{ site.baseurl }}/assets/json/total_book_scans.json" style="width: 100%"></vegachart> 

This current project investigates the outsourcing pattern that the *Scanning Labor* team identified through pairing analysis of scanning metadata records with bills of lading that record the import of goods from overseas suppliers to Internet Archive’s US locations. This project is interested in piecing these two data sources together to understand the infrastructure and workers who have made possible internet archive’s production of culture at scale through visualizing probable connections between suppliers, scanning centers, scanning workers, and the books they digitized. Ultimately, this project is an experiment in computationally-aided critical digital humanities. Through my never certain speculative data visualizations, I attempt to use computational techniques to re-embed IA data in the contexts of its creation, reappraise the work of the people who made it, and through doing so breakdown the black boxing of data, workers, and users that I will suggest culture at scale hinges upon.


# Map 

<vegachart schema-url="{{ site.baseurl }}/assets/json/connections-map.json" style="width: 100%"></vegachart>

# All scans att the centers

<vegachart schema-url="{{ site.baseurl }}/assets/json/outsourced_centers.json" style="width: 100%"></vegachart>


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
