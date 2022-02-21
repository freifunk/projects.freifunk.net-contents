---
name: "Try LibreMesh without having a router"
desc: "Ease the installation of a virtual environemt to try libremesh out"
requirements:
 - "Knowledge or interest in containerization an virtualization tools, such as docker"
difficulty: "medium"
size: "full-time"
status: open
mentors:
 - germanferrero
 - spiccini
initiatives:
 - GSoC
 - GSoC2022
tags:
 - LibreMesh
 - Docker
 - QEMU
collaborating_projects:
 - "LibreMesh"
---

When technical people reach libremesh.org and decide to give it a try, they usually need to go and buy some routers, flash them with a compiled image of LibreMesh firmware, and start digging in to learn what can it do.
This set up a high barrier for new contributors to take their first steps.
As of today, LibreMesh nodes can be set up in a virtual environment using QEMU and wiring the virtual machines to create a virtual mesh network, but these tools need to be taken to a production-ready state. Containerization and CI will be needed to provide a smooth experience for newcomers to "Try it out" LibreMesh right after they visit libremesh.org.

#### Milestones

##### GSOC 2022 COMMUNITY BONDING

* Understand current libremesh virtualization dev tools.
* Define the expected UX. 
* Define the development roadmap.
* Exploration of virtualization & containerization tools limitations.

##### GSOC 2022 MIDTERM

* First cross-platform container image for setting up virtual libremesh network being published.

##### GSOC 2022 FINAL

* Adding entry "Try it out" to libremesh.org web site.
* Continuous Integration to keep newcommers using latest released versions. 
* Document what can be done with the virtual network.
