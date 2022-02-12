---
name: "VXLAN VPN"
desc: "A vxlan base VPN broker"
requirements:
 - "Analyzing code and evaluate solutions"
 - "Implementing a VXLAN-Broker"
 - "Client server code optimasation"
 - "debugging + package building"
difficulty: "medium"
status: open
mentors:
 - 2tata
 - simonkurka
initiatives:
 - GSoC
 - GSoC2021
 - ffnw
 - freifunk
tags:
 - OpenWrt
 - Networking
 - VPN
collaborating_projects:
 - freifunk
---

This project is about implementing a broker for VXLAN (Virtual Extensible LAN) to get a Layer 2 high performance VPN as an alternative to l2tp and fastd in Gluon. Furthermore the VXLAN-VPN-client should be optimized and integrated into the offical OpenWRT Repository. VXLAN-VPN-client code draft: (https://git.ffnw.de/sk/vxlan-vpn-client/-/tree/master)

#### Milestones

* Get familiar with existing code and protocols and start coding
* Implement broker and client, including debudding/testing
* Integrate into OpenWrt documentaion and gluon integration.

##### Preparation

* Get familiar with VXLAN
* Get familiar with gluon (https://gluon.readthedocs.io/en/latest/)
