---
collaborating_projects:
  - libremesh
desc: "Develop NetJSON monitoring agent for LibreMesh."
developers_involved: []
difficulty: medium
status: open
initiatives:
  - GSoC
issues:
markdown: libremesh-netJSON-agent.md
mentors:
  - G10h4ck
  - NicoEchaniz
  - nemesisdesign
name: "LibreMesh NetJSON Agent"
requirements:
  - "Lua programming language"
  - "Almquist shell"
  - "NetJSON"
  - "Software Architecture"
  - "Hardware for testing"
tags:
  - Architecture
  - OpenWrt
  - LibreMesh
  - NetJSON
  - JSON
  - uBus
---


LibreMesh has support for monitoring via LibreMap agent since years, nowadays
NetJSON is emerging as common format to exchange networking information between
community networks actors, since the inception of NetJSON. LibreMesh community
has been supportive of this effort and now that NetJSON gain momentum we think
is the right moment to implement NetJSON based monitoring as a module of
LibreMesh firmware.


#### Milestones

* Create a working testbed network with LibreMesh
* Propose a reasonable architectural solution to address this issue
* Code the proposed solution after discussion with LibreMesh developers
* Test and document the code


##### PREPARATION/BONDING

* Get a general understanding of community networks
* Briefly study LibreMesh networking architecture
* Briefly study LibreMesh software architecture
* Clearly understand NetJSON specification
* Briefly study other NetJSON implementations
* Briefly study other uBus
* Discuss possible development with mentors
* Buy low price compatible devices to operate the test network
