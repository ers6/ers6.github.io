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


Internet Archive announced the launch of its book scanning program with a December 2004 blog [post](https://blog.archive.org/2004/12/15/open-access-text-archives/). The program began as a partnership between Internet Archive and ten academic institutions/libraries across the world in an effort to digitize free, open access versions of books made available to the public via the web. 

Internet Archive sets up scanning centers in partner-institution libraries. They furnish these scanning centers with bespoke book scanning equipment that they refer to as a scribe machine. To scan a book using the scribe machine, a worker places the book between a cradle and a pane of glass. To capture an image of a page, the worker presses a pedal with their foot. This causes the pane of glass and cradle to press together and hold the book steady. Once the movement stops, the scribe machine’s cameras capture an image of the book page. Upon the pedal’s release, the glass pane and book cradle part, the worker turns the next page, and the process repeats ([Hanamura](https://blog.archive.org/2021/02/09/meet-eliza-zhang-book-scanner-and-viral-video-star/)). The number of pages scanned per worker per day varies based on the quality of the book and the pace of the scanning worker, but many people scan between 3,000 to 5,000 pages per day. 

<iframe width="420" height="315" src="https://www.youtube.com/embed/QThaHpkFVzw" frameborder="0" allowfullscreen></iframe>

While Internet Archive celebrates some scanning workers (such as Eliza Zhang featured in the video above) on their blog, the process through which the books are scanned remains opaque. To shed light on how the dynamics of scanning labor in the Internet Archive’s book scanning program over time have changed, I visualized the *Scanning Labor in the Internet Archive*’s dataset. *[Scanning Labor](https://scanninglabor.github.io/IAScanningLabor/index.html)* is a digital humanities project created by Lucian Li, Eleanor Colbert, David Satten-Lopez, and myself that seeks to reappraise the work of scanning workers in the Internet Archive. Through part of this project, we have collected a dataset consisting of 2.5 million records of books scanned by the internet archive between 2004 and 2022. Each scanning record contains information about the date upon which the book was scanned and the name of the scanning center at which the scan was captured. 

While these books make up a small percentage of the total number of books in the Internet Archive, the patterns the records reveal suggest that around 2011 the Internet Archive began outsourcing the majority of its scanning center operations to business process outsourcing firms in east and southeast Asia. In the visual below, for example, spikes in scanning activity appear to correspond with the operation of the scanning centers "Datum Data Co, Ltd.", "Hong Kong", and "Innodata Knowledge Services, Inc." 


<vegachart schema-url="{{ site.baseurl }}/assets/json/total_book_scans.json" style="width: 100%"></vegachart> 


Further investigation reveals that these scanning sites, unlike the others in the dataset, are business process outsourcing firms in the global south. 


<vegachart schema-url="{{ site.baseurl }}/assets/json/geodash.json" style="width: 100%"></vegachart> 

## Works Cited 

"About the Internet Archive." *Internet Archive*, https://archive.org/about/. Accessed 28 April 2023.

Colbert et al. *Scanning Labor in the Internet Archive: Outsourcing and exploitation in mass digitization projects*. 2022, https://scanninglabor.github.io/IAScanningLabor/index.html. 


Hanamura, Wendy. "Meet Eliza Zhang, Book Scanner and Viral Video Star," Internet Archive Blogs, 9 February 2021, https://blog.archive.org/2021/02/09/meet-eliza-zhang-book-scanner-and-viral-video-star/.


Kaplan, Jeff "Open-Access Text Archives," Internet Archive Blogs, 15 December 2004, https://blog.archive.org/2004/12/15/open-access-text-archives/.  
### Sources of Contextual Visuals:

Data for "Types of Content in the Internet Archive on a Log Scale" was extracted from the following pages of the internet archive: 
- http://archive.org/web/
- https://archive.org/details/texts
- https://archive.org/details/audio
- https://archive.org/details/movies
- https://archive.org/details/image
- https://archive.org/details/software 

"Eliza digitizing books at the Internet Archive." Youtube, uploaded by Internet Archive, 2023, https://www.youtube.com/watch?v=QThaHpkFVzw.


## The Data & Analysis

See the analysis used to create the 3 custom data visualizations for this article and the scans per month dataset: 


<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/scanninglabor/IAScanningLabor/main/code/scans_per_center_per_year.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/ers6/ers6.github.io/blob/5a82d5bc2bee32fdc6ab289cf9cbce46d9c6f903/assets/code/final_project_visuals.ipynb" text="The Analysis" %}
</div>

