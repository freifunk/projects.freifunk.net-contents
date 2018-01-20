---
collaborating_projects:
  - libremesh
desc: "Develop librenet6 integration into LibreMesh"
developers_involved: []
difficulty: medium
status: open
initiatives:
  - GSoC
issues:
markdown: libremesh-librenet6-integration.md
mentors:
  - G10h4ck
  - NicoEchaniz
name: "LibreMesh LibreNet6 integrations"
requirements:
  - "Lua programming language"
  - "Software Architecture"
  - "Network Architecture"
  - "Hardware for testing"
tags:
  - Architecture
  - OpenWrt
  - LibreMesh
  - LibreNet6
  - Tinc
  - IPv6
---


LibreMesh already does extensive use of IPv6 technology, we even have an IPv6
mesh tunnel broker provider based on Tinc VPN. It works very well but
configuring the tunnel is a manual work that requires specific skills which are
not common in the majority of communities. Because of this, communities often
are not taking advantage on IPv6 while their routers already support and make
good use of it.
To improve this situation the student should design a semi-automatic system to
grant access to trusted routers to LibreNet6 (this may include key exchange) and
code a tiny LiMe module that take care of tunnel configuration.


#### Milestones

* Create a working testbed network with LibreMesh
* Propose a reasonable architectural solution to address this issue
* Code the proposed solution after discussion with LibreMesh developers
* Test and document the code


##### PREPARATION/BONDING

* Get a general understanding of community networks
* Clearly understand LibreMesh networking architecture
* Clearly understand LibreMesh software architecture
* Discuss possible development with mentors
* Buy low price compatible devices to operate the test network
