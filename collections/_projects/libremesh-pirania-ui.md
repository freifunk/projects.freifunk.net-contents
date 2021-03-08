---
name: "LibreMesh Pirania UI"
desc: "Finish the migration of the LiMe-App's Pirania captive portal administrative interface"
markdown: libremesh-tests.md
collaborating_projects:
  - libremesh
  - altermundi
developers_involved: []
difficulty: medium
status: open
initiatives:
  - GSoC
  - GSoC2021
issues:
mentors:
  - SAn
  - gferrero
  - nicopace
requirements:
  - "Javascript"
  - "ReactJS"
  - "StoryBookJS"
  - "testing"
  - "ubus"
  - "lua"
  - "OpenWRT"
tags:
  - GSoC2021
  - OpenWrt
  - LibreMesh
  - Networking
  - Community Networks
---

Pirania is the mesh captive portal for community networks implemented within LibreMesh.org .
It has gone through a major overhaul, mainly on the router's side, where it became more robust and ready to use.
The User Interface has lagged behind, with an early working implementation that is now broken as the changes have broken backwards compatibility.
This proposal seeks to address this issue, by implementing Pirania's administrative interface on top of the LiMe-app, using the existing code as a base, and benefitting from the late architectural changes done on the LiMe-app.

#### Milestones

##### GSoC Community Bonding

* The student should get familiarized with the development environment
* The student must have a Lime-App repository fork.
* The student must learn how to contribute code via merge request mechanism.
* The student should relate comfortably with the LibreMesh developers.

##### GSOC Midterm

* An initial implementation that has the barebones for interacting with the ubus API.
* Tests implemented for each functionality.
* Storybook.js implementation of screens.
* An in-depth understanding on how it works.

##### GSOC Final

* A complete implementation of the Pirania UI
