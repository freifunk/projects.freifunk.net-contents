---
name: "qaul.net SOCKS Proxy Gateway"
desc: "Develop qaul.net SOCKS Proxy Gateway through Network and IP space discovery"
collaborating_projects:
  - qaul.net
developers_involved: []
difficulty: medium
status: open
initiatives:
  - GSoC
issues: https://git.open-communication.net/qaul/qaul.net/issues/122
markdown: qaul.net_SOCKS-Proxy-Gateway.md
mentors:
  - spacekookie
requirements:
  - "Networking knowledge"
  - "Rust programming language"
tags:
  - GSoC2020
  - qaul.net
  - Rust
  - Networking
---

`qaul.net` is a mesh networking communication app that has been around since 2011
with active users around the world, using it instead of traditional internet
infrastructure to share files, data and communicate.

The project is now undergoing a complete re-write in Rust in order to support
more modern hardware, be more maintainable and extendable.
The rewrite is at the moment in it's alpha state and will become beta during the GSoC project.

We are searching for students who want to be a part of this rewrite, with the idea to become longer term contributers to the project.

A new feature to add to the project would be a socks proxy that acts as a 
gateway from and to the internet (or another TCP/IP network) though the qaul.net network.

The person working on this project will be responsible for creating and implementing
a concept to access qaul.net and its decentralized services via a SOCKS proxy.
The aim is to allow users to be able to communicate and interact with the qaul.net 
network via the SOCKS proxy without having to run the qaul.net protocol.


#### Milestones

* Create the concept for the SOCKS proxy
* Implement the SOCKS proxy
* Ensure, fix and enable all services to run over it.
  * Test the implementation.


##### PREPARATION/BONDING

* Get a general understanding of how qaul.net works
  * Download and build the project.
  * Read the related part of the documentation.
* Take part in the qaul.net developer meetings, project IRC communication and mailing list.
* Get a closer understanding of the qaul.net protocol and services
* Learn about SOCKS proxies
* Discuss possible development with mentors
