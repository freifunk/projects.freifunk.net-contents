---
name: "Steering Clients"
desc: "Steering clients to non-mesh APs"
status: in_review
requirements:
 - C
difficulty: "hard"
mentors:
 - PolynomialDivision
initiatives:
 - GSoC
tags:
 - OpenWrt
collaborating_projects:
 - "OpenWrt upstream"
---

Core-router setups consist of several access points (APs). Some of them have client access wifi, and some also use 802.11s for further meshing. However, the APs that only have client access should be preferred so more resources are available for the 802.11s mesh. That is why a daemon should be written that automatically steers clients to non-mesh APs if the signal strength allows it.

#### Milestones

##### PREPARATION/BONDING

* Understand the radio resource managments 802.11v/k

##### CODING PHASE 1

* Find a way to exchange the needed information between all APs

##### CODING PHASE 2

* Implement the steering

##### CODING PHASE 3

* Bug Fixing