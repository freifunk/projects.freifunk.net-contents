---
collaborating_projects:
  - retroshare
desc: "RetroShare Improve VOIP"
developers_involved: []
difficulty: medium
size: half-time
status: open
initiatives:
  - GSoC
  - GSoC2022
issues:
markdown: retroshare.voip.md
mentors:
  - csoler
name: "RetroShare Improve VOIP"
requirements:
  - "Analyzing and coding"
  - "C++"
  - "Video compression"
tags:
  - GSoC2022
  - video compression
  - video codecs
  - C++
---

Retroshare already offers the possibility to talk using Voice/Video over IP, but
only as a toy system. It currently needs a skilled developer to integrate a
proper cross-platform video codec that would be capable of frame-rate
auto-adjustment and be robust to network delays. This is a challenging project
that needs a good understanding of how existing VoIP works and interacts with
the network layer, as well as a technical understanding of how video compression
works in general.

This project can be a half-time project for a sufficiently skilled developper.

#### Milestones

* find a suitable cross-plaform video codec
* handle auto-adjustment of bandwidth for video/sound with proper priority handling to avoid gaps
* implement proper GUI device selection and notifications

##### PREPARATION/BONDING

* get familiar with the Retroshare network and existing VOIP code
* discuss possible options with the developers
* we only consider recruiting applicants who made a few relevant pull requests to the project first. A good starting point would be to improve the current VOIP graphical user interface.
