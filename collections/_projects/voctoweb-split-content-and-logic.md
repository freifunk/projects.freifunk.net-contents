---
collaborating_projects:
  - freifunk
desc: "Split the project to make it easier to use multiple instances"
developers_involved:
  - andibraeu
difficulty: medium
size: full-time
status: open
email: ab+gsoc2022@andi95.de
initiatives:
  - GSoC
  - GSoC2022
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
  - GSoC2022
  - json
  - web
  - voctoweb
  - video
---

Voctoweb is the software behind media.ccc.de and used for distributing video recordings of a lot of events. We forked their repo to set up our own video portal, [media.freifunk.net](https://media.freifunk.net). As there was only one user of this software for years, content pages and templates are mixed with the logic.

Goal of this project should be: We're able to set up a new instance of voctoweb and add our own contents, designs and templates. Logical parts should be shared (in code) by all instances.

It may be hard to split the original project in a first step. But if we find a way to make it easy for others to customize the installation, that doesn't matter.

## Milestones

### Preparation/Bonding

* Install your own instance of voctoweb and try to understand how it works
* identify the components to separate

### Coding period

* identify the general and the customizable parts
* find ways to apply the customizable parts to a default installation
* improve documentation on installing voctoweb
* add documentation on how to apply and develop customizable parts
