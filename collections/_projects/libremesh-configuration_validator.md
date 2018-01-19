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
  - Architecture
  - OpenWrt
  - LibreMesh
  - Lua
  - RegExp
---


LibreMesh meta-firmware configuration system is highly flexible and powerful,
this is very useful for experienced user, but an uncautious user can easily
write an inconsistent configuration leading to unexpected firmware behaviors, a
specification to define at least syntactic and maybe semantic validators in
modules and a configuration files validator module could be implemented to check
configurations before applying.


#### Milestones

* Create a working testbed network with LibreMesh
* Propose a reasonable architectural solution to address this issue
* Code the proposed solution after discussing with LibreMesh developers
* Test and document the code


##### PREPARATION/BONDING

* Get a general understanding of community networks
* Briefly study LibreMesh networking architecture
* Clearly understand LibreMesh software architecture
* Discuss possible development with the mentors
* Buy some low price compatible devices to operate the test network
