---
name: "Minstrel-TX-Rate-Control_in_Userspace"
desc: "Implement Minstrel Rate Control in Python Userspace based on new mac80211 Linux Kernel relayfs Interface"
collaborating_projects:
  - openwrt.org
developers_involved:
  - thuehn
difficulty: tough
status: open
initiatives:
  - GSoC
  - GSoC2022
issues:
size: full-time
markdown: evernet_minstrel_rate_control_in_userspace.md
mentors:
  - thuehn
requirements:
  - "Python"
  - "Ansi C"
  - "ash"
tags:
  - GSoC2022
  - OpenWrt
  - mac80211
  - Linux Kernel
---

Efficient and fair resource allocation is necessary to deliver services to multiple wifi routers in a mesh network.
The resource `data rate` (e.g. the set of supported MCS rates per STA) and it's dynamic allocation is facilitated by rate control algorithms, which operate at the mac80211 Linux subsystem.

Minstrel_HT [1] is the state-of-the-art and default Linux kernel rate control algorithm in todays access and mesh networks.
The goal of this project is to implement and evaluate the Minstrel_HT rate control algorithm as a Python userspace application over the Evernet Mesh network and therewith create a new userpace rate control API to change/enhance/evaluate new rate control ideas in mesh networks. Based on WiFi components (Mediatek mt76xx & Atheros ath9k chipsets) used in Freifunk mesh routers, this project enables a flexible community-driven development of new rate control ideas in mesh networks, as adaptations are shifted from kernel to user space. The new Rateman API specifically designed to export rate control functions from kernel space to user space via relayfs has been developed as part of the BMBF-funded SupraCoNeX research project [2].
Building on the outcomes of this project our Freifunk community will be able to firstly validate those API, and secondly provide a reference Minstrel_HT implementation in user space to be used for evaluation and adaptation of resource allocation in mesh networks.

#### Resources

* [1] https://blog.cerowrt.org/papers/minstrel-sigcomm-final.pdf
* [2] https://supraconex.de/

#### Milestones

* Flowchart and proposal for Python-based software architecture of Minstrel HT rate control algorithm
* Implementation of Minstrel HT WiFi rate control algorithm as a Python package
* Tests and demo Minstrel_HT operation, along with bug fixes if required
* Definition of WiFi network rate control experiment
* Performance analysis of Minstrel HT in kernel space and user space

##### PREPARATION/BONDING

* Get a general understanding of Minstrel_HT is mac80211 kernel implementation.
* Structure Minstrel_HT's main functions (rate probing, statistical averaging, rate sorting and annotation)

##### Coding Period

* Implement the user space Python variant of Minstrel_HT
* Run validation experiments to compare both, kernel and user space variants
* Work step by step on the list of milestones until the performance evaluation
* Create documentation and a HowTo use the new rate control
