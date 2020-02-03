---
name: "Evernet Software Defined WAN for Multiple Mesh-Uplinks"
desc: "Develop a SD-WAN package for Freifunk/OpenWrt to use multiple uplinks in mesh based WLAN networks."
collaborating_projects:
  - www.evernet-eg.de
developers_involved: []
difficulty: medium
status: open
initiatives:
  - GSoC
issues:
markdown: evernet_SD-WAN_for_multiple_mesh_uplinks.md
mentors:
  - Thomas Hühn (Bluse)
requirements:
  - "ASH shell"
  - "Wireguard"
  - "LUA/JS"
tags:
  - GSoC2020
  - evernet-eg
  - SD-WAN
  - efficient loadbalancing
  - fast failover
---

`Evernet` is a community based rural mesh network based on Freifunk principles organizes as a cooperative since 2008.
Across four villages based in Thueringen/Germany, the Evernet community network
consists of 103 participating households that run an OpenWrt based Freifunk
mesh IEEE 802.11n,ac node on their roof and several OpenWrt based access points
within the house as access technology.
The project consists of a strong technical networking team that focus on a
permanent refresh network infrastructure to support mesh networks as fast as
radio technologies evolve. Therefore the Evernet core network is build on a
dedicated backbone infrastructure between mesh nodes to increase the overall
mesh performance. Those links are based on dedicated 43x 5GHz, 2x 24Ghz and
14x 60GHz point-to-point radio connections that form the Evernet backbone
network. The uplink connectivity for the Evernet mesh is currently realized by
three VDSL lines that span across three villages. In case of an outage of such
an uplink it is up to the routing deamon, currently OLSRd, to handle this.
In this GSoC project we propose a new approach to (1) handle gateway outages
faster and (2) make use of multiple gateway in terms of load-balancing through
an OpenWrt-Linux based Software-Definded-Networking (SD-WAN) attempt.
Once each mesh router has a dedicated Wireguard layer-2 connectivity to each
gateway, there exists the technical possibility to make use of those new tunnel
interfaces to increase robustness of internet connectivity and bandwidth of such
multiple gateway connections.

A person working on this task would be responsible for the creation of a
decentralized deployable Wireguard based tunnel setup and its multiplexing.
This multiplexing could be based on a sufficient configuration or extension to
the mwan3 OpenWrt package. This needs to be evaluated to decide weather the
feasibility of an OpenWrt toolset of available tools is sufficient to build
such a SD-WAN setup or if there are certain parts missing that need to be
developed.


#### Milestones

* Develop technical concept for multi gateway multiplexing
  * What are the Wireguard and Routing challenges to tackle?
  * How will handover switches in cases of failure speed up?
  * Which kind of traffic flows can be easily loadbalanced hence muliuplexed
    across multiple gayteways?
* Create a usable Freinfunk web-based user interface for administration.


##### PREPARATION/BONDING

* Get a general understanding of how multi gateway mesh network work
* Get a general understanding of Wireguard and mwan3
* Learn hoe to combine those technical tunnel and load scheduling and sharing
  technics
* Discuss possible development with mentors
