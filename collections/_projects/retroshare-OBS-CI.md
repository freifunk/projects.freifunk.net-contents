---
name: "RetroShare continuous integration"
desc: "Improve RetroShare continuous integration with tests on many platforms"
markdown: retroshare-OBS-CI.md
collaborating_projects:
  - RetroShare
developers_involved: []
difficulty: medium
status: open
initiatives:
  - GSoC
issues:
mentors:
  - csoler
  - G10h4ck
requirements:
  - "Analyzing and coding"
tags:
  - GSoC
  - C++
  - CI
---


As of today RetroShare continuous integration system is limited to compiling a
subset of the code in TravisCI for MacOS and Linux and on AppVeyor for Windows.
While it is useful to spot compilation error on merge requests,
it is not enough to spot regressions and more subtle compilation errors that
arise only with some compiler version or libraries.
Some testing code is also integrated in RetroShare repository but it is quite
old, outdated and disabled at compile time because it fails to compile.

This project aims to improve this situation, to achieve that some interesting
research and development directions might be:

* Add unit tests taking advantage of modern testing frameworks
* Evaluate if something from the old testing code might be used or if it is
better to drop that completely
* Use Open Build Service (OBS) for testing on multiple linux distributions
* Setup continuous integration for Android
* Investigate if GitlabCI might be helpful
* Use RetroShare JSON API to setup multiple instances and test how they
interoperate

#### Milestones

##### GSoC Community Bonding

* Get familiar with the RetroShare network
* Get familiar with the RetroShare code
* Discuss possible developments options with the developers


##### GSOC Midterm

* To be defined by candidate proposal


##### GSOC Final

* To be defined by candidate proposal
