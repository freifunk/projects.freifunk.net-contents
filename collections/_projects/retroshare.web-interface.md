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
  - "JSON / Mithril"
  - "CSS"
  - "A bit of C++, but not strictly necessary"
tags:
  - GSoC2019
  - Web interface
---

The Retroshare software already has a preliminary web interface, but it covers only the
very basics of the software interactions, and does not benefit from the nice
graphical look it should have.  Furthermore, Retroshare now implements a json API to join the software
internals and the html requests from the web browser, where Json handling code is automatically generated using Doxygen. 

Consequently, the work to develop a modern web interface is limited to designing this interface in javascript (e.g. with Mithril) and 
connecting it to the correct slots in the JSon API.  A bit of C++ undestanding is required to read the API headers, it is not 
needed to be a C++ master to understand how to use the JSON API.

We already provide working test examples of how to call Retroshare internals
through javascript code. We also provide a detailed roadmap and pointers to all required information
in the following file: 
	https://github.com/csoler/RSNewWebUI/blob/master/GSoC_2019.txt

#### Milestones

* implement proper login/passwd handling 
* improve the web UI for file transfers (it is extremely basic now), adding/removing friends, showing internal statistics, etc.
* implement the web UI for configuration options
* implement a nice looking CSS for the web UI

##### PREPARATION/BONDING

* get familiar with the Retroshare network and the existing premature web interface. See the provided basic working examples.
* understand how the current JSon framework works with Retroshare and how it is possible to add new handles if necessary
* discuss roadmap with the developers

Note: acceptance *requires* to complete task 101 of the above roadmap during the bounding period.


