---
collaborating_projects:
  - libremesh
desc: "User friendly interface for LibreMesh ground routing module"
developers_involved: [ gmarcos87 ]
difficulty: medium
status: open
initiatives:
  - GSoC
issues:
markdown: libremesh-ground_routing_web_interface.md
mentors:
  - G10h4ck
  - p4u
name: "LibreMesh ground routing user friendly interface"
requirements:
  - "User Interface Design"
  - "Programming"
  - "Networking"
  - "Hardware for testing"
tags:
  - GSoC2018
  - UIX
  - Networking
  - OpenWrt
  - LibreMesh
  - Community
---


Most mesh networking software has evolved around the simplified model where
each node has WiFi neighbors each of which integrate one or more radios on the
same device. This simplified model has allowed developers to build sensible
abstractions and cost models.
Nowadays most community networks have a relevant number of nodes such that this
assumption is not true anymore. Nodes with far away links are present and often
those nodes feature dedicated devices as "dumb radios". Other nodes end up
having more then one device with
routing protocol installed often with exotic topologies. To work properly and
have reasonable performance those nodes require manual configuration written
by highly skilled people which is not viable for most rural community networks.
To improve this situation some time ago lime-hwd-ground-routing package was
developed and added to LibreMesh offering a more uniform way to configure
those kind of nodes, but this module still requires the user to write UCI
configurations and know the hardware internals to some extent which is not
common knowledge skill in most of our contexts.
In any case, lime-hwd-ground-routing is an important building block to make
community networks more and more self-manageable by non techie people.
We believe that having a good user interface which takes advantage of that
module as back-end would be a huge win for user experience.
Creating that user friendly interface is a welcome proposal for this GSoC.


#### Milestones

* Create a working testbed network with LibreMesh ground routing
* Propose a reasonable user interaction to configure ground routing
* Propose a solution integrable with one of the existing LibreMesh UI
* Design the interface
* Test and document the interface and the code


##### PREPARATION/BONDING

* Get a general understanding of community networks
* Understand how LibreMesh works from the user perspective
* Understand LibreMesh networking architecture
* Understand LibreMesh software architecture
* Discuss possible development with mentors
* Buy low price compatible devices to operate the test network
