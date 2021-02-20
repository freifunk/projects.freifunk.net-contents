---
name: "OpenWrt eBPF/XDP Support"
desc: "Development of a eBPF/XDP loader and development environment for OpenWrt"
collaborating_projects:
  - www.openwrt.org
developers_involved: []
difficulty: high
status: open
initiatives:
  - GSoC
  - GSoC2021
issues:
markdown: openwrt_ebpf_support.md
mentors:
  - schuza
requirements:
  - "C"
  - "LUA/JS"
tags:
  - GSoC2021
  - OpenWrt
  - network debugging
  - efficient loadbalancing
  - network analytics
---

`OpenWrt` is a distribution for embedded devices such as WiFi router etc.
The goal is to ease tasks such as network debugging, obtaining device statistics,
or performing performance measurements etc. `eBPF` and eXpress Data Path `XDP`
allow to load functionality into the Linux kernel during runtime.
A person working on this task would be responsible for the creation of a
an easy to use toolchain and loader for OpenWrt-based routers. Moreover, the
project also aims to perform a brief evaluation of eBPF and XDP on different system
architectures such as ARM, MIPS, x86, AMD64. Additionally, the project should
also provide a brief set of examples for running on OpenWrt-based devices for
purposes such as network debugging, traffic filtering, and network analytics.


#### Milestones

* Develop technical concept for the devleopment environment for eBPF and XDP on OpenWrt
* Development of a cross compile eBPFs and XDP for OpenWrt
* Development of a eBPF and XDP loader for OpenWrt
* Development of different eBPF and XDP use cases
* Performance evalution on different platforms


##### PREPARATION/BONDING

* Get a general understanding of how eBPF and XDP works
* Get a general understanding of how the OpenWrt development environment works
* Get a general understanding of the inner workings of OpenWrt such as ubus, rpcd, uhttpd etc.
* Discuss possible development with mentors
