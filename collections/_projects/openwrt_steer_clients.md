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

Core-router setups consist of one router that is responsible for all the management tasks. The management tasks consist of layer-3-meshing and client management (DHCP). However, this router is connected to a bunch of other routers that are all in the same layer-2 domain and forward the requests or mesh traffic to the core router. Some of the APs have only client access wifi, and some also use 802.11s for further meshing. If clients are connected to APs that are also used for meshing, the other site that is connected via mesh will experience a drop in performance since it has to share its airtime with a bunch of clients. That is why clients should prefer APs that only have client access or APs there no other mesh station is connected to. By doing so, more resources are available for the 802.11s mesh. Since clients do not care about other mesh traffic, we have to steer the clients to other APs. Amendment 802.11v  allows steering a client by sending a bss transition frame. Further, 802.11k allows collecting important information from clients about other APs that are in their range. In the end, a daemon should be written that automatically steers clients to non-mesh APs if the signal strength allows it.

#### Milestones

##### PREPARATION/BONDING

* Understand the radio resource managments 802.11v/k

##### CODING PHASE 1

* Find a way to exchange the needed information between all APs

##### CODING PHASE 2

* Implement the steering

##### CODING PHASE 3

* Bug Fixing
* Documentation