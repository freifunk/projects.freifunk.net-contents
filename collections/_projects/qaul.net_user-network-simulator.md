---
collaborating_projects:
  - qaul.net
desc: "Develop qaul.net user network simulator."
developers_involved: []
difficulty: medium
status: open
initiatives:
  - GSoC
issues:
markdown: qaul.net_user-network-simulator.md
mentors:
  - spacekookie
  - mathjud
name: "qaul.net"
requirements:
  - "Rust programming language"
  - "Software Architecture"
tags:
  - GSoC2019
  - qaul.net
  - Rust
  - Network Simulation
  - Routing Protocol
---

`qaul.net` is a mesh networking communication app that has been around since 2011
with active users around the world, using it instead of traditional internet
infrastructure to share files, data and communicate.

The project is now undergoing a complete re-write in Rust in order to support
more modern hardware, be more maintainable and extendable.
We are searching for students who want to be a part of this rewrite in the
early stage, with the idea to become longer term contributers to the project.

One area of work is a testing platform to abstract over the low-level details 
of the routing protocol to provide an easy way to emulate a working network
for the upper layers of `qaul.net`.
Someone working on this project would not only be responsible for writing this
simulator but also work with the other `qaul.net` developers on core library
internals as well as API decisions affecting the routing protocol module.

The simulator would act as a kind of quickcheck property testing framework for
the rest of the application, while needing to be tested via property testing itself.

#### Milestones

* Develop simulator concept
* Implement simulator
* Run & test the evolving routing protocol
  * Extend the simulator to be able to support this development


##### PREPARATION/BONDING

* Get a general understanding of how qaul.net works
* Get a general understanding of the `libqaul` core APIs
* Learn about property testing
* Discuss possible development with mentors
