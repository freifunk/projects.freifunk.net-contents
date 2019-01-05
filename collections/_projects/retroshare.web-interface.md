---
collaborating_projects:
  - retroshare
desc: "RetroShare port web interface to JSON API"
developers_involved: []
difficulty: easy
status: open
initiatives:
  - GSoC
issues:
markdown: retroshare.web-interface.md
mentors:
  - csoler
  - G10H4ck
name: "RetroShare port web interface to JSON API"
requirements:
  - "Web Development"
  - "JSON"
  - "Capability to read and understand C++"
tags:
  - GSoC2019
  - Web interface
---

The software already has a web interface, but it doesn't look nice and covers
only the very basics of the software interactions, also it is still based on the
deprecated `libresapi` while it should use the new JSON API developed during
2018.
This project is probably the easiest of all related to RetroShare, most of the
work is web design, while a bit of C++ undestanding is required to read the API
headers, it is not needed to be a C++ master to understand how to use the JSON
API.

#### Milestones

* improve the web UI for file transfers (it is extremely basic now), adding/removing friends, showing internal statistics, etc.
* implement the web UI for configuration options
* implement a nice looking CSS for the web UI

##### PREPARATION/BONDING

* get familiar with the Retroshare network and the existing premature web interface
* understand how RetroShare JSON API works
* discuss roadmap with the developers


