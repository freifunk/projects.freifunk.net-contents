---
name: "LibreMesh Tests Major Coverage"
desc: "Contribute to the mainteinability, robustness and ease for contributors of the the LibreMesh project by implementing tests"
markdown: libremesh-tests.md
collaborating_projects:
  - libremesh
  - altermundi
developers_involved: []
difficulty: medium
status: open
initiatives:
  - GSoC
issues:
mentors:
  - (potentially) SAn
  - nicopace
requirements:
  - "lua"
  - "testing"
  - "OpenWRT"
tags:
  - GSoC2021
  - OpenWrt
  - LibreMesh
  - Networking
  - Community Networks
---

The LibreMesh project allows communities to create their own networks by their own means, with little to know prior knowledge required.
It includes the building blocks to build an Operating System for wireless routers for this purpose, and it is based on OpenWRT.
Building on last year's successful GSoC project were it implemented the basis for test-driven development and continuous integration, this year we will increase the bet on it.
This project seeks to increase the amount of modules tested, and the coverage in these modules.
As the process also requires to understand how the different parts work, it will not only add tests but also architectural documentation that can contribute to increase the maintainability of the project.

#### Milestones

##### GSoC Community Bonding

* The student should get familiarized with the development environment
* The student must have a lime-packages repository fork.
* The student must learn how to contribute code via merge request mechanism.
* The student should relate comfortably with the LibreMesh developers.

##### GSOC Midterm

* Essential modules have tests implemented:
  * shared-state
  * first-boot-wizard
  * lime-system
  * ubus-\* packages related to the current lime-app implementation
* each of the modules that have increased in tests, have a documentation that at explains the architecture

##### GSOC Final

* all tested modules have reasonable documentation, explaining what the module does and an explaination of the architecture
* at least half of the repository modules have tests implemented
