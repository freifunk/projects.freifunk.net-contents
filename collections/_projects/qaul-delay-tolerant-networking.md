---
name: "qaul.net Delay Tolerant Routing"
desc: "Develop a Delay Tolerant Routing Extension for RATMAN"
collaborating_projects:
  - qaul.net
  - qaul
developers_involved: []
difficulty: medium
status: open
initiatives:
  - GSoC
  - GSoC2021
issues: https://git.open-communication.net/qaul/qaul.net/-/issues/138
markdown: qaul-delay-tolerant-networking.md
mentors:
  - MathJud
requirements:
  - "Rust"
  - "Routing"
tags:
  - GSoC2021
  - qaul.net
  - "Routing Protocol"
  - DTN
  - peer2peer
---

# Delay Tolerant Routing Extension for qaul.net

**Create a Delay Tolerant Routing extension for the qaul.net routing protocol RATMAN.**

Apart from the classical MANET-Routing (Mobile Adhoc Network) for currently connected devices, a Delay Tolerant Network for not currently reachable devices shall be implemented. In small implementations it shall be played with different concepts of Delay Tolerant Routing.

Delay Tolerant Routing means to send messages and network packages in a store and forward manner to other devices currently connected to the network, that have a higher probability to reach the receiver sooner then the sender or be closer to it.

There are several concepts for delay tolerant routing, such as routing by:

* statistical uptime
* social proximity
* by elected 'guard nodes'


## About qaul.net

`qaul.net` is an ad-hoc wireless mesh networking app to communicate directly with
other users in proximity without any Internet connectivity.
qaul.net interconnects many operating systems and devices via Wifi, Bluetooth and
local networks.
The project started in 2011 and is currently rewritten in the programming language Rust.

qaul.net routes everything in user space and creates an identity based routed overlay network
over all kind of existing networks. The router is called RATMAN (Route and Transaction Manager).
and is heavily inspired by BATMAN.

The scope of this project is to extend the qaul.net routing protocol
RATMAN with delay tolerant behaviour.

qaul.net is developed by the 'Open Community Project Association', is funded by various foundations and is looking for students who want to participate in this GSoC, with the goal of becoming long-term contributors to the
project.

https://qaul.net


#### Milestones

* Study delay tolerant routing protocols.
* Develop a delay tolerant network concept.
* Implement the delay tolerant protocol into qaul.net.
* Test and debug the protocol.


##### PREPARATION/BONDING

* Study mesh networking protocols
* Gain a general understanding of how the qaul architecture works
* Discuss possible development with mentors
