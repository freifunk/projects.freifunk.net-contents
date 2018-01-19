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
  - Pau
name: "LibreMesh ground routing user friendly interface"
requirements:
  - "User Interface Design"
  - "Programming"
  - "Networking"
  - "Hardware for testing"
tags:
  - UIX
  - Networking
  - OpenWrt
  - LibreMesh
  - Community
---


Most of mesh networking software has evolved around the simplified model where
each node has some WiFi neighbor each of them integrating one or more radios
on same device. This simplified model has allowed developers to build sensible
abstractions and cost models.
Nowadays most of the community networks has a relevant amount of nodes were this
assumption is not true anymore. Nodes with far away links are present and often
those nodes feature dedicated devices as "dumb radios" without routing protocol
installed on the latters, other nodes end up having more then one device with
routing protocol installed often with exotic topologies. To work properly and
have reasonable performances those nodes require manual configurations written
by highly skilled persons which is not viable on most of rural community
networks.
To improve this situation some time ago lime lime-hwd-ground-routing package has
been developed and added to LibreMesh offering a more uniform way to configure
those kind of nodes, still this module require the user to write UCI
configurations and know the hardware internals to some extent which is a scarce
skill in most of our contexts.
Anyway lime-hwd-ground-routing is an important building block to make community
network more an more self manageable by non techie people, and we think that
having a good user interface that take advantage of that module as back-end
would be a huge win for user experience.
Creating that user friendly interface is a welcome proposal for this GSoC.


#### Milestones

* Create a working testbed network with LibreMesh ground routing
* Propose a reasonable user interaction to configure ground routing
* Propose a solution integrable with one of the existing LibreMesh UI
* Design the interface
* Test and document the interface and the code


##### PREPARATION/BONDING

* Get a general understanding of community networks
* Understand how LibreMesh works form user perspective
* Understand LibreMesh networking architecture
* Understand LibreMesh software architecture
* Discuss possible development with the mentors
* Buy some low price compatible devices to operate the test network
