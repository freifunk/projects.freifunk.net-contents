---
name: "OpenWrt device page"
desc: "Refresh overview page for OpenWrt supported devices"
requirements:
 - HTML
 - CSS
 - JavaScript
 - YAML
 - Jekyll
 - Hugo
 - Shell
 - CI
difficulty: "medium"
mentors:
 - aparcar
initiatives:
 - GSoC
tags:
 - Website
 - OpenWrt
 - CI
collaborating_projects:
 - "OpenWrt upstream"
---

Create overview of OpenWrt supported devices to simplify user choice of
aquicreing new devices.

#### Milestones

##### PREPARATION/BONDING

* Get an overview of Jekyll/Hugo functionality
* Look at current implementation
  * https://openwrt.org/toh/start
  * https://libremesh.org/docs/hardware/index.html
  * https://wiki.freifunk.net/Freifunk-Firmware_Gluon/Hardware
* Find Freifunk/LibreMesh/etc specific information to be stored (e.g. 802.11s support)
* Understand YAML
* Read trough installation procedures in OpenWrt Wiki ([example](https://openwrt.org/toh/tp-link/tl-wdr3600#installation))
* Join project communication platforms like IRC, forums or mailing lists

##### CODING PHASE 1

* Design hardware overview based on the [forum discussion](https://wiki.freifunk.net/Freifunk-Firmware_Gluon/Hardware).
* Evaluate what views and search filters are usable
  * Request community
* Start merging installation documentation for devices into snippets

##### CODING PHASE 2

* Create templates rendering YAML hardware and installation docs to pages ([example](https://aparcar.github.io/openwrt-devices/devices/tp-link_archer_c20_ac750_v1/))
* Add new OpenWrt design to templates
* Scan trough openwrt.git log and find newly added devices and installation procedures
  * Integrate them into snippets

##### CODING PHASE 3

* Add filter and search functions based on JavaScript
* Setup CI that automatically renders new devices
* Evaluate integration into official OpenWrt website
