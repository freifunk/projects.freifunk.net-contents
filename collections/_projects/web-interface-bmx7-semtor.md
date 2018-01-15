---
name: "BMX7 Semtor Web Interface"
desc: "Create easy to use web interface for bmx7 sentor protocool"
requirements:
  - "Analyzing and coding"
  - "html, javascript, json"
difficulty: medium
issues:
  - ""
mentors:
  - axn
initiatives:
  - GSoC
tags:
  - json
  - web
  - mesh
  - bmx6
  - bmx7
collaborating_projects:
  - libremesh
  - freifunk
status: open
---

The popular routing protocol bmx6 evolved to bmx7 and gained a important new
feature: The newly introduced protocol *semtor* is able build a web of trust
between nodes in a mesh. Only trusted nodes are used for routing while unknown
or distrusted notes are ignored.

While this feature already works there is currently now easy way for end-users
to configure it. A possible approach would be to combine bmx7
[NetJson](http://netjson.org/docs/index.html) output with the JavaScript
framework [d3](https://d3js.org/). 


#### Milestones

* Show the bmx7 network graph in a web interface. Possible choices could be
  * [luci](https://github.com/openwrt/luci)
  * [luci-ng](https://github.com/jow-/luci-ng)
  * [lime-app](https://github.com/libremesh/lime-app)

* Clickable nodes 


##### PREPARATION/BONDING

* Install a minimal bmx7 setup for testing
* Choose a web interface and understand how to add modules
* Read about the NetJson standard
