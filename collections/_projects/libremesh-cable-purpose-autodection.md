---
name: "LibreMesh Cable Purpose Autodection"
desc: "For the router to detect if you are connecting a client, another router, an internet connection, and to configure itself accordingly at runtime"
markdown: libremesh-cable-purpose-autodection.md
collaborating_projects:
  - libremesh
  - altermundi
developers_involved: []
difficulty: medium
size: "350 hours"
status: disabled
initiatives:
  - GSoC
  - GSoC2023
issues:
mentors:
requirements:
  - "Lua programming language"
  - "Networking Knowledge"
  - "Software Architecture"
  - "Hardware for testing"
tags:
  - GSoC
  - GSoC2023
  - OpenWrt
  - LibreMesh
  - Networking
  - Community Networks
---

When a community network router ethernet port is acting as a gateway to the
Internet or as a border to neighboring networks, the network configuration
usually needs to be changed from the default settings to accommodate for the
specific role.
A router ethernet port can be connected to the Internet, or connected to a dummy
wifi device for a point to point link, or connected to another router of the
same mesh network to expand mesh coverage.
All these cases would benefit of specific configuration. As of today handling
those configuration manually represents a barrier for communities without
technical experts who could understand and optimize the devices ethernet ports
configuration appropriately.
Most of the described situation could be detected at runtime through automatic
tests and the required configuration applied automatically, the goal of this
project is to develop the software needed to accomplish automatically to the
described needs.


#### Milestones

##### GSoC Community Bonding

* The contributor should enumerate all ethernet cable setups that might be needed.
* The contributor must have a LibreMesh repository fork.
* The contributor must learn how to contribute code via merge request mechanism.
* The contributor should relate comfortably with the LibreMesh developers.
* The contributor should individuate one or more real world community network and establish a fluid cooperation relationship with them.


##### GSOC Midterm

* Autodetection of all the possible scenarios of cable connections.
* A package should be ready to be tested on community networks.


##### GSOC Final

* Deployment of the package in all the nodes of the chosen community network.
