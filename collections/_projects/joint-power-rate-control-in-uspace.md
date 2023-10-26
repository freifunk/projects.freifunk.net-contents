---
name: "Joint Power and Rate Control in User space for Freifunk OpenWrt Mesh & Access Networks"
desc: "Developing a WiFi resource allocation algorithm in user space which exploits both transmission rates and power levels."
status: completed
requirements:
 - Python
 - Linux
 - C
difficulty: "tough"
size: "350 hours"
issues:
mentors:
 - thuehn
 - schuza
initiatives:
 - GSoC
 - GSoC2023
tags:
 - Joint Rate and Power Control
 - OpenWrt
 - User space
 - GSoC2023
collaborating_projects:
 - openwrt.org
 - supraconex.de
---

The performance of IEEE 802.11 (WiFi) networks has been far from optimal, especially when multiple participants share the same channel in an uncoordinated manner. These wireless devices are limited to operating only within the unlicensed ISM band, and consequently, a critical component that determines the throughput of WiFi networks is resource allocation algorithms. Most of these algorithms rely on only one transmission parameter to adapt to the changing wireless environment, such as transmission rates [1] or power levels [2].

In Linux-based devices, the resource allocation is handled in the mac80211 kernel subsystem, restricting the development of such algorithms to the kernel space, which has its limitations and challenges. With this in mind, recent advancements at SupraCoNeX [3] have enabled annotation of transmission rate and power level from user space for Linux-based OpenWrt [4] access points, permitting precise control over the wireless transmission from user space. This capability has eased the research on resource allocation for better management of interference and a potential increase in spatial reuse, especially in a highly dense network. Therefore, this project aims to develop a joint resource allocator [5] in user space to increase aggregate throughput in WiFi mesh and access networks running on OpenWrt OS.

#### Resources

* [1] [Introduction to Rate Control](https://blog.freifunk.net/2022/06/13/minstrel-tx-rate-control-in-user-space-gsoc-22/) & [Minstrel HT Source](https://git.kernel.org/pub/scm/linux/kernel/git/torvalds/linux.git/tree/net/mac80211/rc80211_minstrel_ht.c?id=8415816493b7589e74ff4e1e7eaf3aadc7b73621)
* [2] [Introduction to Transmit Power Control](https://ieeexplore.ieee.org/abstract/document/6952281)
* [3] [SupraCoNeX Research](https://supraconex.de/)
* [4] [OpenWrt Project](https://openwrt.org/)
* [5] [Minstrel-Blues: A Joint Rate & Power Controller](https://github.com/thuehn/Minstrel-Blues)

#### Milestones

##### GSOC COMMUNITY BONDING

* Understand transmission rates and power levels in IEEE 802.11 networks.
* Learn about rate control and transmit power control in Linux.
* Study Minstrel-Blues to understand how a joint resource allocator works.
* Familiarize with the user space API and Python packages from SupraCoNeX.

##### GSOC MIDTERM

* Implement a simple rate and power control for desk experiments with complete documentation.
* Test and validate transmit power control for mt76 and ath9k driver.
* Concrete formulation of the final joint rate and power control with proper evaluation.
* Create diagram/s to depict the software architecture of the proposed joint rate and power control.

##### GSOC FINAL

* A working joint rate and power control with complete documentation and execution guide as a SupraCoNeX Github repository.
* Ready to run demo scripts to showcase the potential of the joint rate and power control.
