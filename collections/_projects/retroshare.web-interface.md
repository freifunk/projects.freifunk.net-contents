---
collaborating_projects:
  - retroshare
desc: "Improve existing Retroshare web interface"
developers_involved: []
difficulty: easy
status: completed
initiatives:
  - GSoC
issues:
markdown: retroshare.web-interface.md
mentors:
  - csoler
  - G10Hack
name: "Improve existing Retroshare web interface"
requirements:
  - "Analyzing and coding"
  - "C++"
  - "CSS"
  - "JSon/Qt"
tags:
  - GSoC2018
  - Web interface
---

The software already has a preliminary web interface, but it covers only the
very basics of the software interactions, and does not benefit from the nice
graphical look it should have. This project is probably the easiest of all,
since the software already implements a partial json API to join the software
internals and the html requests from the browser, but it still represent a lot
of work as the software currently offers a lot of GUI handles in its Qt version
that would need to find an equivalent functionality in the web interface
version.

#### Milestones

* improve the web UI for file transfers (it is extremely basic now), adding/removing friends, showing internal statistics, etc.
* implement the web UI for configuration options
* implement a nice looking CSS for the web UI

##### PREPARATION/BONDING

* get familiar with the Retroshare network and the existing premature web interface
* understand how the current JSon frame work works with Retroshare
* discuss roadmap with the developers


