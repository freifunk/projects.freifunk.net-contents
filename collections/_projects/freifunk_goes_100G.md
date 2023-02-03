---
name: "Freifunk Fiber Backbone over 100G"
desc: "Running Freifunk Fiber Backbone Links via Mellanox 100G Switches on OpenWrt"
collaborating_projects:
  - openwrt.org
developers_involved:
  - schuza
difficulty: midrange
status: open
initiatives:
  - GSoC
  - GSoC2023
issues:
size: "350 hours"
markdown: freifunk_goes_100G.md
mentors:
  - schuza
  - thuehn
requirements:
  - "Ansi C"
  - "ash"
tags:
  - GSoC2023
  - OpenWrt Build Env
  - Linux Kernel
---

Current Freifunk Community networks accross Europe are expanding their wireless P2P backbone infrastruture to wired fibre links, hence capacities beyond 10GBit/s are achieveable.
Today's switching hardware can be categorised into three design aproaches:
    - Switch Abstraction Interface (SAI) [1] which is leveraged by SONiC (NOS) [2] 
    - OF-CONFIG [3] which enables to configure the forwarding plane of Broadcom-based switches
    - Switchdev (Linux kernel API [4]), which could be leveraged by the Distributed Switch Architecture (DSA) [5]

Moreover, other approaches exist to expose the packet handling/forwarding into the user space
 - DPDK/VPP interface that would require a significant re-emplementation of the Freifunk network stack and features such as olsrd/batman/babel routing deamons. The flexible switchdev Linux kernel API builds upon standard Linux tools such as IP etc. this enables Freifunk communities to code as well as add features running atop a classical Linux-based system also on devices beyond 10 Gbps interfaces. Since NVIDIA Mellanox Spectrum II switches implement the Linux kernel switchdev API, they seem to be a reasonable choice to achieve this goal.

Accordingly, the goal of this project is to port Freifunk/OpenWrt [6] OS to the Mellanox Spectrum II-based switch[7] hardware - in such a way, that the ONIE [8] bootloader triggers an OpenWrt boot, daemons such as olsrd/batman/babel routing deamons can run as usual, and (Q)SFP-based ports are deployable on fiber links.

#### Resources

* [1] https://github.com/opencomputeproject/SAI
* [2] https://azure.github.io/SONiC/
* [3] https://github.com/openvswitch/of-config
* [4] https://www.kernel.org/doc/html/latest/networking/switchdev.html
* [5] https://www.kernel.org/doc/Documentation/networking/dsa/dsa.txt
* [6] https://openwrt.org/
* [7] https://github.com/Mellanox/mlxsw/wiki
* [8] https://opencomputeproject.github.io/onie

#### Milestones

* DTS Integration for at least Mellanox Spectrum II-based switches in OpenWrt
* add new OpenWrt "Mellanox" target with ONIE bootloader support
* SFP+ p2p 100G link setup test on desk

##### PREPARATION/BONDING

* Understanding of the OpenWrt build environment
* Understanding of the different Switching-based Architectures such as switchdev, SAI, OF-CONFIG
* Understanding of ONIE and Linux OS bring-up process

##### Coding Period

* Porting Meallanox Switch with Sectrum II chipset to OpenWrt
* Add dedicated Mellanox target to the Freifunk/OpenWrt device set
* Evaluation 100G SFP+ fiber ports
