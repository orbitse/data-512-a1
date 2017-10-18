# data-512-a1: DATA 512 Assignment 1

### __Goal of Project__
  To analyze views of English Wikipedia pages from 2008 - 2017. This README file contains information to reproduce the analysis, including data descriptions, attributions and provenance information, and descriptions of all relevant resources and documentation (inside and outside the repo) and hyperlinks to those resources.
  
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
 - List any known issues or special considerations with the data that would be useful for another researcher to know.
 - For example, you should describe that data from the Pageview API excludes spiders/crawlers, while data from the Pagecounts API does not.

### __API Documentation__
The Wikipedia page view data came from two APIs: Pagecounts API and Pageviews API. 
 - The legacy __Pagecounts API__ ([documentation](https://wikitech.wikimedia.org/wiki/Analytics/AQS/Legacy_Pagecounts), [endpoint](https://wikimedia.org/api/rest_v1/#!/Pagecounts_data_(legacy)/get_metrics_legacy_pagecounts_aggregate_project_access_site_granularity_start_end)) provides access to desktop and mobile traffic data from January 2008 through July 2016.
 - The __Pageviews API__ ([documentation](https://wikitech.wikimedia.org/wiki/Analytics/AQS/Pageviews), [endpoint](https://wikimedia.org/api/rest_v1/#!/Pageviews_data/get_metrics_pageviews_aggregate_project_access_agent_granularity_start_end)) provides access to desktop, mobile web, and mobile app traffic data from July 2015 through September 2017.

### Final Data File: en-wikipedia_traffic_200801-201709.csv
Describe the values of all fields in your final data file.

