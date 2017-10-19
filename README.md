# data-512-a1: DATA 512 Assignment 1

### __Goal of Project__  

  The goal is to follow best practices for open scientific research while constructing, analyzing, and publishing a dataset of monthly traffic on the pages in English Wikipedia from July 1, 2008 through September 30, 2017. The resulting project should contain enough information to be fully reproducible by others: from data collection to data analysis.  

  This project documents (1) the combination of Wikipedia traffic data from two different Wikimedia REST API endpoints into a single dataset, (2) the data wrangling steps necessary to consolidate five JSON files into a single CSV file, and (3) the visual analysis of the clean data.  

  This README file contains the information needed to reproduce the analysis, including a description of the data and all relevant resources and documentation, with hyperlinks to those resources.  
  
### __About Data__
 - The Wikipedia page view data used in this analysis was provided under an [Apache 2.0 License](http://www.apache.org/licenses/LICENSE-2.0).
 
 Copyright 2017 Erin Orbits

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

 - For more information, see the Wikimedia Foundation terms of use [LINK](https://wikimediafoundation.org/wiki/Terms_of_Use/en). 
 
### __Data Issues__
 - issues or special considerations with the data that would be useful for another researcher to know.  

### __API Documentation__
The Wikipedia page view data came from two APIs: Pagecounts API and Pageviews API. 
 - The legacy __Pagecounts API__ ([documentation](https://wikitech.wikimedia.org/wiki/Analytics/AQS/Legacy_Pagecounts), [endpoint](https://wikimedia.org/api/rest_v1/#!/Pagecounts_data_(legacy)/get_metrics_legacy_pagecounts_aggregate_project_access_site_granularity_start_end)) provides access to desktop and mobile traffic data from January 2008 through July 2016.
 - The __Pageviews API__ ([documentation](https://wikitech.wikimedia.org/wiki/Analytics/AQS/Pageviews), [endpoint](https://wikimedia.org/api/rest_v1/#!/Pageviews_data/get_metrics_pageviews_aggregate_project_access_agent_granularity_start_end)) provides access to desktop, mobile web, and mobile app traffic data from July 2015 through September 2017.  
 The Pageview API gives you the ability to exclude traffic from spiders and crawlers, by setting the agent parameter to agent = user. While the older Pagecount API does not allow you to filter by agent. 

### Final CSV Data File: en-wikipedia_traffic_200801-201709.csv
The columns in the combined CSV file include: year, month, pagecount_all_views, pagecount_desktop_views, pagecount_mobile_views, pageview_all_views, pageview_desktop_views, and pageview_mobile_views.  
  - pagecount_all_views = pagecount_desktop_views + pagecount_mobile_views
  - pagecount_desktop_views = the monthly views of the main English Wikipedia pages from Jan. 2008 through July 2016
  - pagecount_mobile_views = the monthly views of the mobile version of the English Wikipedia pages from Jan. 2008 through July 2016
  - pageview_all_views = pageview_desktop_views + pageview_mobile_views
  - pageview_desktop_views = the monthly views by people rather than bots or web crawlers of the main English Wikipedia pages from July 2015 through Sept. 2017
  - pageview_mobile_views = the monthly views by people rather than bots or web crawlers of both the mobile English Wikipedia pages and via the mobile app from July 2015 through Sept. 2017


  

