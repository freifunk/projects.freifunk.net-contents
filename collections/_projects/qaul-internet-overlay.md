---
name: "qaul internet overlay driver"
desc: "Develop (& refactor) a new qaul internet overlay driver"
collaborating_projects:
  - qaul
developers_involved: []
difficulty: medium
status: open
initiatives:
  - GSoC
issues: https://git.qaul.org/qaul/qaul/-/issues/2
markdown: qaul-internet-overlay.md
mentors:
  - spacekookie
requirements:
  - "Rust"
  - "TCP/UDP Networking"
  - "Data structures"
  - "Optional: QUIC"
  - "Optional: Nix"
tags:
  - GSoC2021
  - qaul
  - Networking
  - "High performance"
---

`qaul.net` is an ad-hoc wireless mesh networking app, and development
framework created in 2011 and used by various activists and projects
around the world.  Its aim is to make it easier to bring internet/
network access to places that currently don't have any, and to connect
participants in a network together directly when no other
infrastructure is available.

Since 2019 the project has been undergoing a complete re-write in Rust
in order to support modern mobile hardware, and provide a more
flexible architecture that other developers can use to write
applications on-top of.

We are searching for students who want to participate in this
re-write, with the goal of becoming long-term contributors to the
project.

The qaul router architecture is network interface agnostic, and
requires drivers to translate the internal routing scheme (based on
ed25519 public keys) and an arbitrary address space (such as ipv6).
There are already several network drivers available.

The scope of this project is to refactor two of the existing drivers
(TCP and UDP) into a single "overlay" driver, which can utilise either
TCP or UDP.  Optionally QUIC can be evaluated as an alternative for
TCP connections.


#### Milestones

* Create a general mapping structure from qaul routing IDs (pubkeys) to IP addresses
  * Handle all corner cases around new peers, connection drops, and re-connects.
  * Write a comprehensive set of tests to ensure this core functionality
* Implement bi-directional connection logic
  * Used for peers that are "equal" in terms of firewall access
  * No server, no client
  * Can be used with UPNP when available
* Implement uni-directional connection logic
  * Used when one peer can't be reached directly
  * Implicit "server" to connect to
  * Implicit "Client" uses reverse-connection channel
* Corner case: handle true uni-directional links
  * (i.e. uni-directional antenna wifi antenna)
* Develop a test suite for this driver
  * Unit tests
  * Simple integration tests
  * Complex network tests with virtial machines (mechanism is available via our build system)


##### PREPARATION/BONDING

* Gain a general understanding of how the qaul architecture works
* Study the existing networking drivers
* Discuss possible development with mentors
