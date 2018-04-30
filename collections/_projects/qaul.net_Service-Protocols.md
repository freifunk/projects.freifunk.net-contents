---
collaborating_projects:
  - qaul.net
desc: "Integrate qaul.net Service Protocols in an network independent manner"
developers_involved: []
difficulty: high
initiatives:
  - GSoC
status: in_progress
issues:
  - "https://github.com/qaul/qaul.net/issues/209"
markdown: qaul.net_Service-Protocols.md
mentors:
  - MathJud
name: "Integrate Service Protocol"
requirements:
  - "Analyzing and coding"
  - "Mathematical models network analyzation and neighbour finding"
  - "C"
  - "Real-Live testing of implementation"
tags:
  - GSoC2018
  - C
  - NetworkAnalyzation
---

Historically all service and user discovery functions were implemented via the OLSR plugin, the broadcasting mechanism as well made use of the network functions of OLSR.

To make qaul.net app usable in every network, you should write an abstraction as well as implementations for different types of networks.

Define a strategy for the neighbor finding for every Implementation.

Abstractions:
* User Discovery
* Service Discovery
* Message Flooding (1 to all messaging)

Implementations:
* OLSR (from existing qaul.net implementation)
* Freifunk Networks without OLSR
* Any SOHo Network

To decide wether your implementation really works, you should test your implementation in the existing Freifunk networks.


#### Milestones

* Defining User/Service-Discovery Algorithms
* Implementing the service abstraction layer
* Porting the existing OLSR implementation
* Writing SOHo Network implementation
* Writing Freifunk Network implementation
* Testing implemented Algorithms in real existing networks

##### PREPARATION/BONDING

- Analyzing and current qaul.net Service Protocols
- Searching the best Algorythems for the Task
