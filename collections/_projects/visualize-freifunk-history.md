---
collaborating_projects:
  - freifunk
desc: "Use historic data from our freifunk API to visualize freifunk's history"
developers_involved:
  - andibraeu
difficulty: medium
size: "175 hours"
status: open
email: ab+gsoc2023@andi95.de
initiatives:
  - GSoC
  - GSoC2023
issues:
  - "https://github.com/freifunk/vis.api.freifunk.net/issues/1"
  - "https://github.com/freifunk/vis.api.freifunk.net/issues/15"
markdown: visualize-freifunk-history.md
mentors:
  - andibraeu
name: "Visualize freifunk community data and history"
requirements:
  - "Analyzing and coding"
  - "data mining"
  - "data visualization"
  - "graphQL"
  - "R, Python, html, javascript"
tags:
  - GSoC2023
  - json
  - web
  - data mining
---

With our [freifunk API](https://api.freifunk.net/) we collect data from our communities. This data is used to display for example:
* a map of communities
* collect information like events and news
* an overview of donation pages
* aggregate community news to a feed
* aggregate community events to a common calendar
* collect information of nodes and create another map

But there's a lot more data, that's not used anymore. On top of this, we saved this data hourly for nearly 9 years now. So it would be possible to create timelines and nice visualisations about freifunk communities.

## Milestones

### Preparation/Bonding

* explore data collected by freifunk API
* find possible cases for visualisation
* find useful cases for time-based visualisations

### Coding period

* create a service to import and transform freifunk API data
* build a web page that can visualize data, allow to embed single visualisations on other pages
* introduce a general way on how to create new visualisation
* write documentation on how to create new queries and visualisations for non-programmers
* bonus: add an API to this service to query freifunk API data
