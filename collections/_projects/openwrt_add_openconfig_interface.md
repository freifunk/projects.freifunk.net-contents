---
name: "OpenWrt OpenConfig Support"
desc: "Development of an OpenConfig interface for OpenWrt"
collaborating_projects:
  - www.openwrt.org
developers_involved: []
difficulty: high
status: open
initiatives:
  - GSoC
issues:
markdown: openwrt_add_openconfig_interface.md
mentors:
  - schuza
requirements:
  - "C"
  - "LUA/JS"
tags:
  - GSoC2021
  - OpenWrt
  - Open Networking
  - configuration
  - OpenConfig
  - network management
---

`OpenWrt` is a distribution for embedded devices such as WiFi router etc.
The goal is to ease tasks such as network configuration and integration 
into heterogeneous environment with open networking hardware.
`OpenConfig` is an interface for vendor-neutral, model-driven network 
management and builts on top of YANG.
The goal is to build an OpenConfig-based interface for OpenWrt network 
devices such as WiFi access points or switches. 
A person working on this task would be responsible for the creation of an
OpenConfig-based interface and to integrate it into the OpenWrt environment 
including the integration with uci, ubus etc.
Moreover, the project also aims to create a YANG model for some OpenWrt-based
WiFi access points.

#### Milestones

* Develop technical concept for the OpenConfig interface and OpenWrt system environment
* Development of a OpenConfig Interface
* Development of a YANG-based models for some WiFi access points
* Evalution on the OpenConfig interface


##### PREPARATION/BONDING

* Get a general understanding of how OpenConfig works
* Get a general understanding of how YANG models work
* Get a general understanding of the inner workings of OpenWrt such as ubus, rpcd, uhttpd etc.
* Discuss possible development with mentors
