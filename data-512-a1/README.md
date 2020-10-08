# Human Centered Data Science - A1 Data Curation

This project combine data about Wikipedia page traffic from two different [Wikimedia REST API](https://www.mediawiki.org/wiki/Wikimedia_REST_API) endpoints into a single dataset, perform some simple data processing steps on the data, and then analyze that data via ploting time-series data.

## Data Source
I have used two APIs for collecting wikipedia page views as mentioned below:
1. [The Legacy Pagecounts API](https://wikitech.wikimedia.org/wiki/Analytics/AQS/Legacy_Pagecounts)
2. [The Pageviews API](https://wikitech.wikimedia.org/wiki/Analytics/AQS/Legacy_Pagecounts)

## Features
1. This project contain reusable code to query wikipedia traffic data via api calls and output into json folder.
2. The json files are combined and cleaned and dumped into csv folder for further analysis.
3. The time-series chart is plotted to show traffic over time by differenct access sites such as dekstop, mobile and overall.

## Final Visualization
![Wikipedia Page View Trend](wikipedia%20pageview%20trend%20over%20time%20plot.png)

## Installation

### Main Requirements
* [Python](https://www.python.org/)- version 3.6
* Before installing we recommend setting up a clean [virtual enironment](https://docs.python.org/3.6/tutorial/venv.html).
  

