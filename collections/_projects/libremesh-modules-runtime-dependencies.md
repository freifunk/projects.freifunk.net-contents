---
collaborating_projects:
  - libremesh
desc: "Develop runtime dependencies support for lime-system modules."
developers_involved: []
difficulty: medium
size: "350 hours"
status: disabled
initiatives:
  - GSoC
issues:
markdown: libremesh-modules-runtime-dependencies.md
mentors:
  - G10h4ck
  - altergui
name: "lime-system: Modules Runtime Dependencies"
requirements:
  - "Lua programming language"
  - "Software Architecture"
  - "Hardware for testing"
tags:
  - Architecture
  - GSoC2018
  - OpenWrt
  - LibreMesh
---


LibreMesh meta-firmware aims to be highly modular, and in fact almost all parts
it consist of are split into modules. Some modules depends at run-time on the
fact that another module has already run, nowadays this condition is not
guaranteed and depends on how configuration files are written, but this imply
that an user can break things involuntarily.
Implementing a run-time dependency check system would avoid troublesome
situations, it have to be light, fast, and simple keeping in mind that will be
installed on embedded devices with as little as 4MB of flash.


#### Milestones

* Create a working testbed network with LibreMesh
* Propose a reasonable architectural solution to address this issue
* Code the proposed solution after discussion with LibreMesh developers
* Test and document the code


##### PREPARATION/BONDING

* Get a general understanding of community networks
* Briefly study LibreMesh networking architecture
* Clearly understand LibreMesh software architecture
* Discuss possible development with mentors
* Buy low price compatible devices to operate the test network
