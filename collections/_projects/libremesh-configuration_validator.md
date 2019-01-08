---
collaborating_projects:
  - libremesh
desc: "Develop configuration validation support for lime-system."
developers_involved: []
difficulty: medium
status: open
initiatives:
  - GSoC
issues:
markdown: libremesh-configuration_validator.md
mentors:
  - G10h4ck
  - NicoEchaniz
name: "lime-system: Configuration Validator"
requirements:
  - "Lua programming language"
  - "Software Architecture"
  - "Hardware for testing"
  - OpenWrt
tags:
  - GSoC2018
  - Architecture
  - OpenWrt
  - LibreMesh
  - Lua
  - RegExp
---


The LibreMesh meta-firmware configuration system is highly flexible and
powerful. This is very useful for an experienced user, but an incautious user
can easily write an inconsistent configuration leading to unexpected firmware
behaviors. A specification to define at least syntactic and maybe semantic
validators in modules and a configuration files validator module could be
implemented to check configurations before applying.


#### Milestones

* Create a working testbed network with LibreMesh
* Propose a reasonable architectural solution to address this issue
* Code the proposed solution after discussion with LibreMesh developers
* Test and document the code


##### PREPARATION/BONDING

* Get a general understanding of community networks
* Briefly study LibreMesh networking architecture
* Clearly understand LibreMesh software architecture
* Discuss possible development with mentors
* Buy low price compatible devices to operate the test network
