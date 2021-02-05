---
name: "Freifunk Digital Twin - test on your virtual mesh before going productive"
desc: "Before maintaining your productive mesh - update, migrate  and troubleshoot within your virtualized Freifunk mesh"
collaborating_projects:
  - www.evernet-eg.de
developers_involved: []
difficulty: sporty
status: open
initiatives:
  - GSoC
issues:
markdown: evernet_digital_Freifunk_twin.md
mentors:
  - thuehn
requirements:
  - "Qemu based virtualised OpenWrt VM"
  - "Linux namespaces and networking"
  - "Routing protocols (OLSR, Babel)"
  - "Scripting (Bash, Python, ect.)"
  - 'Git with hooks and CI integration"
tags:
  - GSoC2021
  - Freifunk Evernet e.G.
  - Efficient sys-upgrade testing per target
  - Testing syntax migration changes
  -
---

`Evernet` is a community based rural mesh network based on Freifunk principles organizes as a cooperative since 2008.
Across five villages based in Thueringen/Germany, the Evernet community network
consists of 110 participating households that run an OpenWrt based Freifunk
mesh IEEE 802.11n,ac node on their rooftops and several OpenWrt based access points
within the house as access network. The Evernet core network is build on a dedicated backbone
infrastructure (5GHz, 24GHz & 60GHz P2P links) between mesh nodes to increase the overall performance.
Our Freifunk mesh is driven by a strong technical networking team. It is focused on a
constant maintained network infrastructure and OpenWrt software state following current trunk.
The maxim to keep the  mesh as fast as radio technologies evolves does involve a cyclic 
upgrade and update process. Currently this includes just a smoke test with a set
of targets placed on a desktop. We follow the pace of OpenWrt trunk development
with the goal and commitment to help finding and fixing kernel/driver/config
issues and bugs. Especially those that appear on our Freifunk mesh routers while
transmitting real WiFi user traffic do lack efficient tools for testing and
troubleshooting before going productive with a new Freifunk OpenWrt image. There
is a strong need from the Freifunk community to extend the OpenWrt CI, hence the
digital Freifunk mesh twin GsoC project is born and consists of the following parts:

-fresh compiled OpenWrt trunk images as Qemu VMs (one per target)
-hwsim as WiFi connectivity mac80211 layer
-represent productive mesh nodes by count and inter connectivity in the generated
virtual network twin matching a productive Freifunk mesh state
-fetch topology from real mesh routing state
-translate real mesh topology in a vitual digital twin topology (qemu bridge, Linux namespaces)
-sysupgrade your digital Freifunk mesh twin first
-functional tests on each virtual node, e.g.:
  -mesh, lan & uplink connectivity (routing state)
  -migrate syntax changes in uci config variables

We are looking for students that like to enhance the Freifunk OpenWrt systems
in terms of automated system testing aka CI in a virtual copy of a real mesh.

#### Milestones

* Develop technical concept to transform the real mesh topology, connectivity and 
hardware target state to a digital twin with VM hosts and network setup based on Qemu
  * What are the virtualisation challenges to tackle?
  * How to collect a representative connectivity graph from routing deamon?
  * Design an extendable test cases creation to allow easy extension by other Freifunk communities


##### PREPARATION/BONDING

* Get a general understanding of how Qemu, Linux Namespaces, and virtualization with OpenWrt works
* Get a general understanding of mesh topology fetching from routing deamins (e.g. OLSR v1)
* Learn how to combine those technical virtualisation tools to duplicate real mesh topology to a comparable digital copy that serves as an additional upgrade/update testbed
* Discuss possible development with mentors
