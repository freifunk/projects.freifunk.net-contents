---
collaborating_projects:
  - freifunk
desc: "Split the project to make it easier to use multiple instances"
developers_involved:
  - andibraeu
difficulty: medium
status: open
email: ab+gsoc2018@andi95.de
initiatives:
  - GSoC
issues:
  - "https://github.com/freifunk/voctoweb/issues/2"
markdown: voctoweb-split-content-and-logic.md
mentors:
  - andibraeu
  - christian-draeger
name: "VocToWeb: Split contents and logic"
requirements:
  - "Analyzing and coding"
  - ""
  - "refactoring, migrations"
  - "ruby, html, javascript"
tags:
  - json
  - web
  - voctoweb
  - video
---

Voctoweb is the software behind media.ccc.de and used for distributing video recording of a lot of events. We forked their repo to set up our own video portal, [media.freifunk.net](https://media.freifunk.net). As there was only one user of this software for years, content pages and templates are mixed with the logic.

Goal of this project should be: We're able to set up a new instance of voctoweb and add our own contents. Logical parts should be shared (in code) by all instances.

#### Milestones

##### PREPARATION/BONDING

- Install your own instance of voctoweb and try to understand how it works
- identify the components to separate
