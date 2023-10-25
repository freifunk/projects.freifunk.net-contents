---
name: "Automation tools for LibreMesh firmware build and monitoring"
desc: "Automate the compilation system, configuration and monitoring of LibreMesh using Ansible. Integrate with its web interface Lime-App"
status: completed
requirements:
 - "Analyzing and coding"
 - "Prometheus"
 - "Grafana"
 - "Ansible"
 - "OpenWrt"
 - "lua, bash"
 - "publish code and doc"
 - "report the process"
difficulty: "medium"
size: "350 hours"
issues:
 - "https://github.com/coala/coala/issues/####"
mentors:
 - digitigrafo
 - ilario
initiatives:
 - GSoC
 - GSoC2023
tags:
 - GSoC2023
 - LibreMesh
collaborating_projects:
 - "LibreMesh"
---

Create a set of automated tasks to install services on a Raspberry Pi to meet the needs of small community-network with an administration/tech team, e.g. a set of commonly needed monitoring tools, such as Prometheus, Prometheus-node-exporter, Blackbox-exporter, Altermanager, Grafana, VPN and an editing map service.

Similar projects or packages:
https://gitlab.com/librerouter/miniserver
https://github.com/libremesh/lime-packages/tree/master/packages/altermundi-grafana

The use case is a growing fragmented network with islands of nodes and users; but with a collective management having an overarching vision on what is happening in the network and giving feedback to the users by the [Lime-App](https://github.com/libremesh/lime-app). 

Create a set of Ansible roles to replicate the OpenWrt build-system, to speed-up the process of self-building images for OpenWrt and/or LibreMesh for newcomers, and to easily setup a dedicated machine, with the possibility to later extend the process of build to other automated tasks, like a pub-keys-exchange needed for configuring a VPN, or to update documentations or a webapp.
The Ansible roles would include tasks to build for: different architectures and targets; different OpenWrt and LibreMesh versions; keeping trace of devices with particular needs and related patches; keeping a local list of supported targets; provide a basic functionality to setup a VPN. This should also provide a main configuration file for each device, and the use of the main configuration tools available on LibreMesh, like +/etc/config/lime-*+ and especially +lime-macaddress+ files, "generic-uci-config, lime-asset" functionalities, and configurations and packages provided by community [network-profiles](https://github.com/libremesh/network-profiles) or local packages.
These will be published and shared also on Ansible Galaxy or similar repository as a standalone project.

#### Milestones

* Automation on LibreMesh build system
* Automation on monitoring
* Collectors of data
* Data visualization
* Integration in Lime-App

##### GSOC COMMUNITY BONDING

* Getting familiar with LibreMesh compilation using the OpenWrt buildroot
* Learn to develop a basic LibreMesh package and compile it in a firmware image
* Flashing of at least 3 wifi routers with the compiled LibreMesh
* Have these routers connected in a (indoor) mesh network
* Get familiar with the LibreMesh web interface "Lime-App"
* Get familiar with the OpenWrt basic folders structure and acquainted with its command line interface
* Get familiar with the tools for quantifying the quality of single wireless links, both the ones provided by the Linux kernel and the ones from the router protocols employed in LibreMesh (Batman-adv, Babeld)
* Deploying the already existing monitoring systems on at least 1 Raspberry-Pi
* Document the entire process at least with a post on the Freifunk blog

##### GSOC MIDTERM

* Develop automation on LibreMesh build system
* Write and publish sets of configuration management on Ansible Galaxy
* Deploying automated LibreMesh build system on at least 2 computers
* Publish a "LibreMesh observer" deploy instruction for Arm architecture
* Set up multiple observation points, including at least 2 Raspberry-Pi, to collect data from LibreMesh routers
* Verify if it is possible to integrate a Grafana dashboard in Lime-App to receive feedback about traffic and develop a basic demonstrator
* Write a post on the Freifunk blog detailing which of the monitoring tools under development are suited for being integrated with the LibreMesh web interface "lime-app" and documenting the proof-of-concept integration of Grafana in Lime-App, if achieved
* Propose in the LibreMesh repositories the pieces of code that are standalone

##### GSOC FINAL

* Develop automation on LibreMesh build system
* Write and publish sets of configuration management on Ansible Galaxy
* Deploying automated LibreMesh build system on at least 2 computers
* Publish a "LibreMesh observer" deploy instruction for Arm architecture
* Set up multiple observation points, including at least 2 Raspberry-Pi, to collect data from LibreMesh routers
* Verify if it is possible to integrate a Grafana dashboard in Lime-App to receive feedback about traffic and develop a basic demonstrator
* Write a post on the Freifunk blog detailing which of the monitoring tools under development are suited for being integrated with the LibreMesh web interface "lime-app" and documenting the proof-of-concept integration of Grafana in Lime-App, if achieved
* Propose in the LibreMesh repositories the pieces of code that are standalone


