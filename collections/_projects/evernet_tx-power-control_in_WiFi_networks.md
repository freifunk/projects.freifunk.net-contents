---
name: "TX-Power Control in WiFi Networks"
desc: "Implement per Packet Transmission Power Control for Mediathek and Atheros WiFI chips in OpenWrt"
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
size: "350 hours"
markdown: evernet_tx-power-control_in_WiFi_networks.md
mentors:
  - thuehn
requirements:
  - "Ansi C"
tags:
  - GSoC2022
  - OpenWrt
  - mac80211
  - mt76
  - ath9k
  - Linux Kernel
---

Per packet, hence per client transmit power control, done by each WiFi
router or access point individually, does promise a significant gain in
sum-network throughput in our Freifunk community networks.
The option to transmit WiFi packets at different power levels needs
(a) WiFi chipsets able to change per packets amplifications, (b) a control
interface to make those hardware allocations accessible by its Linux driver
and (c) an mac80211 algorithm that make use of this resource allocation
control knob efficiently.

Dated back to 2007, Atheros IEEE 802.11a/b/g/n chipsets driven by ath5k and
ath9k Linux drivers did first and Mediatek joint recently by hw support for
tx-power control.
The goal of this project is to implement the missing three-tier software parts:
(1) mac80211 structs to annotate per packet tx-power levels
(2) mac80211 structs to account tx-power status information once transmitted
(3) transmit power control (TPC) API for TPC algorithms [1]
-

#### Resources

* [1] 'A Measurement-Based Joint Power and Rate Controller for IEEE 802.11
Networks', http://dx.doi.org/10.14279/depositonce-3725

#### Milestones

* Implementation of new mac80211 status and control structures to annotate
  and account tx-power settings per WiFi packet
* Tackle the Linux upstream process to get it kernel integrated
* Enable tx-power per packet support for mt76 IEEE 8021.11ac drivers
* Validate this new transmit power control per packet feature

##### PREPARATION/BONDING

* Get familiar with the Linux mac80211 per packet function call path
* Identify space and place for adding our new tx-power per packet annotation
* Set-up a OpenWrt router to STA setup for testing/validation

##### Coding Period

* Propose an efficient tx-power per packet annotation mac80211 struct
* Implement this new struct in the mac80211 Linux subsystem
* Enable Mediatek mt76 driver to make use of the newly added tx-power struct
* Run validation experiments
* Create documentation on how to use and test it further
