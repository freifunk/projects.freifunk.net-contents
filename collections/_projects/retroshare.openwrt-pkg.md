---
collaborating_projects:
  - retroshare
desc: "RetroShare OpenWRT package"
developers_involved: []
difficulty: medium
status: open
initiatives:
  - GSoC
issues:
markdown: retroshare.openwrt-pkg.md
mentors:
  - amuuza
name: "RetroShare OpenWRT package"
requirements:
  - "Analyzing and coding"
  - "Reading C++"
  - "Makefile"
tags:
  - GSoC2019
  - OpenWRT
  - Decentralized Internet
---

Retroshare is a friend-to-friend application. As it can work within the LAN, it is specially useful for community networks.

In a Retroshare network, as there is not any central server which is always online, users need to find an online friend-node to route their traffic. Having an always-on Retroshare node would let routing and asynchronous communication happen smoothly.

If there were a CLI Retroshare package for OpenWRT which could basically act as a relay, administrators of community routers could run that package into their routers. That Retroshare software would basically require routing and friendship management capabilities.

That would let Retroshare users -connected to that node- have their traffic routed as if they were in a client-server architecture, without having to install any additional always-on dedicated hardware.

Equally, this package will be useful for those Retroshare users on the Internet who run their own OpenWRT router.

#### Milestones

* Understanding Retroshare
* Analysing resource limits of a home router
* selecting required Retroshare functionalities

##### PREPARATION/BONDING

* Get familiar with Retroshare
* Discuss possible options with the developers

