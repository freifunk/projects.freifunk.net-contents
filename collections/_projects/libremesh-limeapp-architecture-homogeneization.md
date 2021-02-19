---
name: "LibreMesh LiMe-App architecture homogeneization"
desc: "Contribute to the mainteinability and ease for contributors of the LiMe-App by cleaning the system and implementing tests"
markdown: libremesh-limeapp-architecture-homogeneization.md
collaborating_projects:
  - libremesh
  - altermundi
developers_involved: []
difficulty: medium
status: open
initiatives:
  - GSoC
issues:
mentors:
  - gferrero
  - nicopace
requirements:
  - "React"
  - "React-query"
  - "RxJs"
  - "Testing"
tags:
  - GSoC2021
  - OpenWrt
  - LibreMesh
  - Networking
  - Community Networks
  - web
---

The LiMe-App has grown to be a valuable tool for laypeople members of community networks as their prefered tool for maintaining the infrastructure they rely on.
It's development has gone over a series of stages were diferent tools were applied, but as it grew in features it also grew in complexity.
Some of this complexity came naturally as part of its size. There is some coplexity that came through generational changes that were not applied fully yet, were architectural changes were done but not implemented throughout the whole project.
This proposal seeks to invite you to address this by:
- Collectively agree on the set of tools that will be used in the project
- Implement tests that help ensure that general functionality will not be affected through the process, and would enable validation that the process goes in the right direction
- Write a strategy on how to do the migration
- Apply the strategy one plugin at a time
- Document the architecture

#### Milestones

##### GSoC Community Bonding

* The student should get familiarized with the development environment
* The student must have a LiMe-app repository fork.
* The student must learn how to contribute code via merge request mechanism.
* The student should relate comfortably with the LibreMesh developers.

##### GSOC Midterm

* The proposed architecture should be documented
* A strategy on how to do the migration should be in place
* One plugin should have been PR'd with tests passing


##### GSOC Final

* At least 4 plugins migrated
