---
name: "nodewatcher: Build system rework and package upstreaming"
desc: "Rework and simplification of firmware-core build system and package upstreaming"
requirements:
 - "Understanding of OpenWrt build system, Docker and general Linux build tools"
status: in_progress
difficulty: "medium"
mentors:
 - mitar
initiatives:
 - GSoC
tags:
 - GSoC2018
 - nodewatcher
collaborating_projects:
 - wlanslovenija
---
Nodewatcher currently uses Dockerized OpenWrt firmware builders which are manually generated.
Currently their generation is slow and complicated which does not allow quick bug fixing.
They are configured here:https://github.com/wlanslovenija/firmware-core

Packages that are crucial to functioning of Nodewatcher configured nodes are mostly not upstreamed and are also compiled with the OpenWrt source code.

Idea of this is to simplify and speed up the whole building process.
While we are at it also upstream all necesary packages to ease their maintnance.

Student should have experience with the OpenWrt source code and build system, basic knowledge of using Docker and experience with the common Linux build tools,most notably make.

#### Milestones

* Study OpenWrt build system in depth.
* Study firmware-core Docker based build system in depth to spot areas which to improve
* Study firmware-packages-opkg to see which packages are needed (https://github.com/wlanslovenija/firmware-packages-opkg)
* Simplify the build system
* Upstream crucial packages
* After review merge changes
