---
collaborating_projects:
  - libremesh
desc: "Develop BattleMesh testbed based on LibreMesh."
developers_involved: []
difficulty: medium
status: open
initiatives:
  - GSoC
issues:
markdown: libremesh-battlemesh_testbed.md
mentors:
  - G10h4ck
  - Gui
  - Pau
name: "LibreMesh based Battle Mesh testbed"
requirements:
  - "Lua programming language"
  - "Software testing"
  - "Hardware for testing"
  - "Software Architecture"
tags:
  - Architecture
  - OpenWrt
  - LibreMesh
  - BattleMesh
---


In latest years to collect relevant data at Wireless Battle Mesh has been an
hard challenge and in some cases a failure. A relevant part of WBM community
agrees that not having a well tested firmware for the testbed has been a major
hindrance to successful testing and data collection.
Past tentatives of creating a testbed based on WiBed have failed too, apparently
due to lack of maintenance.
While LibreMesh hasn't been designed with testbeds in mind, thanks to its high
modularity and flexibility troughs years it has gained most of the needed
features for a testbed firmware, as a plus it is actively maintained by a
conspicuous and heterogeneous developers community from different community
networks in the world that participate to WBM, all propitious factors for a
satisfactory GSoC project development.


#### Milestones

* Create a working testbed network with LibreMesh
* Complete the implementation of lime-proto-babeld
* Prepare compilation profiles for lime-sdk for each test
* Document how to use the created firmware images to run scientifically valuable tests
* Document how to extend testbed to collect new kinds of data
* Document how to add support for testing of new protocols
* Simulate a WBM test and publish the data
* Eventually create lime-proto modules for new protocols that need testing
* Eventually demonstrate progress at next WBM


##### PREPARATION/BONDING

* Get a general understanding of community networks
* Get a general understanding of Wirelss Battle Mesh
* Briefly study LibreMesh networking architecture
* Clearly understand LibreMesh software architecture
* Discuss possible development with the mentors
* Buy some low price compatible devices to operate the test network
