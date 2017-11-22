---
collaborating_projects:
  - freifunk
desc: "Implement Mikrotik MetaRouter Images to LEDE/Gluon"
developers_involved: []
difficulty: medium
status: open
initiatives:
  - GSoC
issues:
markdown: freifunk_miktorik_metarouter.md
mentors:
  - johannesrudolph
name: "Mikrotik MetaRouter architecture"
requirements:
  - "Analyzing and coding"
  - "identify components that must be changed"
  - "refactoring, migrations"
tags:
  - c
  - firmware
---

Implement / Convert the MiktoTik Patch (https://wiki.mikrotik.com/wiki/Manual:Metarouter) from OpenWRT to LEDE. The MetaRouter Images can for example on the MikroTik RB 3011. 
This is a powerful Router. With this Image for the MetaRouter it is possible to run multiple Virtual Routers on One Device.
At the End the MetaRouter architecture should be integrated in LEDE and in Gluon as well.

#### Milestones

##### PREPARATION/BONDING

- Get Familar with LEDE Contributing Guidelines (https://lede-project.org/submitting-patches)
- found the components that need to migrated or refactored
