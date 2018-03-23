---
name: "Tunneldigger: support for connecting over IPv6 networks"
desc: "Implement support for connecting clients to Tunneldigger VPN servers over IPv6."
requirements:
 - "Python, networking/IPv6 experience."
difficulty: "medium"
mentors:
 - kostko
initiatives:
 - GSoC
tags:
 - GSoC2018
 - nodewatcher
collaborating_projects:
 - wlanslovenija
---

[Tunneldigger](https://dev.wlan-si.net/wiki/Tunneldigger) is a VPN solution used in many community/mesh networks to connect nodes which do not have a wireless link between them into a common network. It uses existing network connectivity (like Internet) between nodes to create L2TP tunnels between them. Current limitation is that those tunnels use only IPv4 and cannot be established over IPv6. (Tunnels are layer 2 and can carry both IPv4 and IPv6 traffic already. The issue here is that they themselves cannot be established over IPv6.)

The aim of the GSoC project is to design and implement IPv6 support for Tunneldigger so that it works in IPv6-only and IPv4/IPV6 mixed environment where both server and client have IPv6 connectivity in some form. Student should have experience or be willing to learn Python and C, compiling and running code for OpenWRT, have experience with networking stack (IPv4, IPv6, NAT).

#### Milestones

* Learn about Tunneldigger.
* Deploy a test network locally using Docker to experiment with Tunneldigger.
* Add IPv6 connectivity to your test network.
* Implement support for IPv6 connections in Tunneldigger.
* Document and implements tests.
