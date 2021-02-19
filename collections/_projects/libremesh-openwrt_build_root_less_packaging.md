---
collaborating_projects:
  - libremesh
desc: "LiMe OpenWrt build-root-less package generator"
developers_involved: []
difficulty: medium
status: in_review
initiatives:
  - GSoC
issues:
markdown: libremesh-openwrt_build_root_less_packaging.md
mentors:
  - G10h4ck
  - nicopace
name: "LiMe OpenWrt build-root-less package generator"
requirements:
  - "Shell programming"
  - "Software Architecture"
  - "Software Packaging"
tags:
  - GSoC2019
  - Architecture
  - OpenWrt
  - LibreMesh
---


To contribute to LibreMesh most of the time one have to create a new module that
is usually shipped as an OpenWrt package. People that have been joining
LibreMesh development over time have been encountering a steep learning curve
expecially packaging their modules, because of the complexity of OpenWrt
build-root. Those packages most of the time consists just of a couple of Lua or
shell scripts that doesn't need cross-compiling and other advanced features
provided by OpenWrt build-root.

Providing a tool to create simple `opkg` archives without depending on the
build-root in those cases would help new developers to start contributing
without a steep learning barrier. Moreover such a tool would have much less
requirements that the OpenWrt build-root.


#### Milestones

* Understand what is exactly an OPKG archive (compression, manifest...)
* Create a simple prototype of the out-of-build-root packager
* Test it with simple packages
* Complete the implementation, and test it with LibreMesh modules
* Document how to use the created tool


##### PREPARATION/BONDING

* Get a general understanding of LibreMesh
* Get a general understanding of OpenWrt
* Briefly study LibreMesh networking architecture
* Clearly understand LibreMesh software architecture
* Discuss possible development with mentors
