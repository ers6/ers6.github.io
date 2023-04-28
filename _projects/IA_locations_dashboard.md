---
name: Where Are the Books from the Internet Archive Scanned? 
tools: [Python, HTML, vega-lite]
image: assets/pngs/cars.png
description: This is a "showcase" project that uses vega-lite for interactive viz!
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---

# Where Are the Books from the Internet Archive Scanned? 
By Elizabeth Schwartz 

## What's the Internet Archive? 

In a former Christian Science church in San Francisco, petabytes of servers store thousands of cassettes, millions of books, and billions of web pages. Welcome to the Internet Archive. Founded in 1996 by a dot com era billionaire, Brewster Kahle, the Internet Archive initially aimed to archive all of the world wide web. 27 years later in 2023, the Internet Archive is now the world’s largest free digital library boasting over 800 billion webpages, 37 million books, 15 million audio recordings, 9.7 million videos, 4.6 million images, and 983 thousand software programs. 

<vegachart schema-url="{{ site.baseurl }}/assets/json/ia-contents-bar-chart.json" style="width: 100%"></vegachart> 

With the exception of the 800 billion webpages--which can be archived by computer programs without much human intervention--all other content in the Internet Archive has been digitized by human workers. This article investigates the processes through which the second most common content type, books, are scanned and added into the Internet Archive’s database. 



## Book Scanning in the Internet Archive


Internet Archive announced the launch of its book scanning program with a December 2004 blog post.(https://blog.archive.org/2004/12/15/open-access-text-archives/). The program began as a partnership between Internet Archive and ten academic institutions/libraries across the world in an effort to digitize free, open access versions of books made available to the public via the web. 

Internet Archive sets up scanning centers in partner-institution libraries. They furnish these scanning centers with bespoke book scanning equipment that they refer to as a scribe machine. To scan a book using the scribe machine, a worker places the book between a cradle and a pane of glass. To capture an image of a page, the worker presses a pedal with their foot. This causes the pane of glass and cradle to press together and hold the book steady. Once the movement stops, the scribe machine’s cameras capture an image of the book page. Upon the pedal’s release, the glass pane and book cradle part, the worker turns the next page, and the process repeats (https://blog.archive.org/2021/02/09/meet-eliza-zhang-book-scanner-and-viral-video-star/). The number of pages scanned per worker per day varies based on the quality of the book and the pace of the scanning worker, but many people scan between 3,000 to 5,000 pages per day. 
https://www.youtube.com/watch?v=QThaHpkFVzw 


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

