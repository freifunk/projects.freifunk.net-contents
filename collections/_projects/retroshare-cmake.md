---
name: "RetroShare port build system to CMake"
desc: "RetroShare build system have grouwn old and plenty of patches, even Qt is now moving away from Qmake toward CMake, times for porting to CMake has come for RetroShare too"
markdown: retroshare-cmake.md
collaborating_projects:
  - RetroShare
developers_involved: []
difficulty: medium
status: open
initiatives:
  - GSoC
issues:
  - https://github.com/RetroShare/RetroShare/pull/999
  - https://github.com/RetroShare/RetroShare/pull/1304
mentors:
  - csoler
  - G10h4ck
requirements:
  - "Analyzing and coding"
tags:
  - GSoC
  - C++
  - Qt
  - Qmake
  - CMake
---


Current RetroShare build system is based on Qmake. Both for RetroShare
historical reasons and for Qmake awkwardness it is diffucult to maintain the
current build system, also adding new features or integrate with new libraries
is quite painfull.
With recent decision from Qt to switch to CMake as it's main build system the
last reason to stay with Qmake have disappeared.
The project aim is to rewrite RetroShare build system with CMake.

#### Milestones

##### GSoC Community Bonding

* Get familiar with the RetroShare network
* Get familiar with the RetroShare code
* Discuss possible developments options with the developers


##### GSOC Midterm

* To be defined by candidate proposal


##### GSOC Final

* To be defined by candidate proposal
