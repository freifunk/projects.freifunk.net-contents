---
name: "Traffic Monitoring and Classification via XDP/eBPF"
desc: "Realization of a traffic monitoring and classification solution via XDP/eBPF"
collaborating_projects:
  - openwrt.org
developers_involved:
  - schuza
difficulty: tough
status: open
initiatives:
  - GSoC
  - GSoC2022
issues:
size: "350 hours"
markdown: traffic_monitoring_and_classification.md
mentors:
  - schuza
requirements:
  - "Ansi C"
  - "Ansi C++"
  - "ash"
tags:
  - GSoC2022
  - OpenWrt
  - XDP
  - eBPF
  - machine learning
  - Linux Kernel
---

Today's network incorporate a wide range of different devices such as laptops, smartphones, IoT devices such as cleaning robots etc. However, the devices might come with different requirement in terms of throughput, connections, latency etc. The goal is to leverage XDP [1] and/or eBPF [2] for the analysis and classification of traffic to perform optimization for the transmission rate control running in the mac80211 subsystem of the Linux Kernel or to built the foundation for networking research such as detecting malicious behavior of devices.

The goal of this project is, to realize traffic monitoring and classification mechanisms via XDP/eBPF that can leverage XDP/eBPF to run within the Linux Kernel on OpenWrt devices [3]. This would enable optimization such as passing the knowledge directly to the transmission rate control to optimize the selected rates, sampling, and latency to the transmission power control. Moverover, the approach should also allow to provide the foundation for further research in the direction of network research.

#### Resources

* [1] https://www.iovisor.org/technology/xdp
* [2] https://ebpf.io/
* [3] https://openwrt.org/


#### Milestones

* Analysis of different approaches to run XDP and eBPF on OpenWrt devices
* Integration of the tools and drivers into OpenWrt
* Design of a moonitoring environment that builds upon the approaches of XDP and eBPF
* Description of different use cases that leverage the capabilities of XDP/eBPF on OpenWrt devices
* Implementation of a dedicated use case that demonstrates the benefits of the XDP/eBPF

##### PREPARATION/BONDING

* Understanding of the OpenWrt build environment
* Understanding of XDP and eBPF

##### Coding Period

* Evaluation of XDP/eBPF on different hardwarew plattforms such as x86, ARM, and MIPS
* Implementation of different XDP and eBPF approches
* Implementation of differnet user space tools as loader
* Evaluation of the use case such as exporting a traffic matrix for further analysis
* Demonstration of the benefits
