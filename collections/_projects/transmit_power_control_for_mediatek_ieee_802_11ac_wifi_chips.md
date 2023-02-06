---
name: "Transmit Power Control for Mediatek IEEE 802.11ac WiFi Chips"
desc: "Developing and testing Transmit Power Control for Mediatek IEEE 802.11ac (VHT) WiFi Chips"
collaborating_projects:
  - openwrt.org
devlopers_involved:
  - thuehn
difficulty: tough
status: open
initiatives:
  - GSoC
  - GSoC2023
issues:
size: "350 hours"
markdown: transmit_power_control_for_mediatek_ieee_802_11ac_wifi_chips.md
mentors: thuehn
requirements:
  - "Ansi C"
tags:
  - GSoC2023
  - OpenWrt
  - Linux Kernel
  - mac80211
  - mt76
---

Transmit Power Control (TPC) is a promising technique to optimise WiFi networks by intelligently adjusting the transmit power of WiFi interfaces to reduce interference and increase overall throughput in wireless networks with multiple members. Being part of ongoing research, it promises to achieve some remarkable enhancements in combination with rate control (RC). Some WiFi chips, in particular from vendors Atheros and Mediatek, allow to annotate the transmit power per packet or even per multi-rate-retry (MRR) stage.
The mac80211 subsystem in the Linux kernel already includes support for coarse-grained TPC which allows to set the transmit power per virtual interface or per station. In the former GSoC 2022 project for TPC [1], support for fine-grained TPC in the mac80211 subsystem of the Linux kernel was proposed and is currently under discussion to be included upstream. It also includes a proof-of-concept implementation for TPC support in the ath9k driver. However, ath9k are end-of-life products with decreasing usage.

The goal of this project is to push TPC further by two means, based on the results of the previous GSoC project:
* extend driver support for fine-grained TPC to mt7603 and mt7615 driver for Mediatek WiFi hardware
* implement a joint RC and TPC algorithm in the Linux kernel based on [2], [3]

-

#### Resources

* [1] https://blog.freifunk.net/2022/09/10/final-gsoc22-report-tx-power-control-in-mac80211/
* [2] https://doi.org/10.14279/depositonce-3725
* [3] https://github.com/thuehn/Minstrel-Blues

### Milestones

#### Preparation/Bonding

* gather deep understanding of mt76 tx-control and tx-status path
* get in touch with existing RC (Minstrel-HT) and proposed TPC algorithms

#### Coding Period

* develop an implementation of TPC support in mt76’s tx-control and status path
* extend Minstrel-HT to have support for TPC
* implement a TPC algorithm in Minstrel-HT to have a joint RC and TPC algorithm
* evaluate TPC on mt7603 and mt7615 WiFi hardware
* submit patches to Linux Kernel development mailing lists