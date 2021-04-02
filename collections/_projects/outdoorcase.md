---
name: "Open Source outdoor cases for off the shelf wireless routers"
desc: "Design and evaluate water proof cases for routers frequently used for Freifunk deployments"
requirements:
 - "CAD"
difficulty: "medium"
status: open
mentors:
 - aparcar
initiatives:
 - GSoC
tags:
 - freifunk
 - case
 - outdoor
 - router
 - cad
---

For better connectivity it makes sense to deploy Freifunk and mesh router
outside. However,commonly used Freifunk devices like *[TP-Link
841/3600/4300](https://openwrt.org/toh/hwdata/tp-link/tp-link_tl-wdr4300)* and
newly released devices like the
*[youhua-wr1200js](https://openwrt.org/toh/hwdata/youhua/youhua_wr1200js) only
come with indoor cases. Devices specialized for outdoor purposes are usually
more expensive, like the various Ubiquiti devices, e.g. the *[NanoStation
Loco2](https://openwrt.org/toh/hwdata/ubiquiti/ubiquiti_nanostation_loco2)*.

A cheap solution could be to design individual cases for frequently used
devices. The router board would be extracted from the original case and
installed into the 3D-printed outdoor case. The case should be designed in a way
to support *[external antenna
connectors](https://www.amazon.de/Eightwood-Externe-Antenne-Bluetooth-Wirelesse-2-RP-SMA-Kabel/dp/B0719HS21N/ref=sr_1_12?s=computers&ie=UTF8&qid=1542738659&sr=1-12&keywords=rp-sma)*
, guard power and Ethernet adapters from rain and be easily mountable to walls
and bars.

The goal would be a selection of 3-4 design for different devices, maybe even a
single case fitting for various router board shapes. A pictured manual per
router to extract and install the board should also be added. All created CAD
files should be available online on platforms like
[thingiverse](https://www.thingiverse.com/) for further modification and
improvement.

#### Milestones

* Figure out popular Freifunk devices
* Extract boards and design one or multiple cases
* Create a manual on how to create and use cases
* Test the cases outside.
