---
name: "WiFi device clustering and fingerprinting"
desc: "Realization of an approach to perform WiFi device clustering and fingerpriting"
collaborating_projects:
  - openwrt.org
developers_involved:
  - schuza
difficulty: tough
status: open
initiatives:
  - GSoC
  - GSoC2023
issues:
size: "350 hours"
markdown: wifi_device_clustering_and_fingerprinting.md
mentors:
  - schuza
requirements:
  - "Ansi C"
  - "Ansi C++"
  - "ash"
  - "Python"
tags:
  - GSoC2023
  - OpenWrt
  - statistics
  - mac80211
  - Linux Kernel
---

The goal is to create an environment that allows to collect rate control and client capabilities to optimize transmission rate control for client devices. To this end, the project will leverage an interface provided by the supraconex [1] project to collect transmission rate statistics from OpenWrt-based [2] devices. Moreover, the system should also allow to leverage fingerprinting mechanisms based on the client capabilities such as WiFi taxonomy [3].

Within the project, both approaches are combined to perform a client-based clustering of WiFi devices to create an understanding whether used rates etc. might correlate between different classes of devices. This should allow to further optimize transmission rate algorithms in the presence of handovers etc. Accordingly, a measurement environment needs to be proposed that allows to anonymously collect statistics from different home networks.

#### Resources

* [1] https://supraconex.de/
* [2] https://openwrt.org/
* [3] https://github.com/NetworkDeviceTaxonomy/wifi_taxonomy

#### Milestones

* Planing of the integration of different mechanisms into the OpenWrt build environment
* Integration of the tools and drivers into OpenWrt
* Design and description of a measurement environment
* Implementation of the measurement environment and necessary tools
* Evaluation of the collected statistics

##### PREPARATION/BONDING

* Understanding of the OpenWrt build environment
* Understanding of statistics
* Understanding of WiFi such as transmission rate control and capabilities

##### Coding Period

* Implementation of different tools
* Integration of the tools and APIs into OpenWrt
* Ralization of the measurement environment
* Collection of privacy-preserving statistics
* Evaluation of the use case

