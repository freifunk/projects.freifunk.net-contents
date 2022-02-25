---
collaborating_projects:
  - retroshare
desc: "Improve the functionality of the existing Retroshare Android client"
developers_involved: []
difficulty: medium
size: "175 hours"
status: open
initiatives:
  - GSoC
  - GSoC2022
issues:
markdown: retroshare.android_client.md
mentors:
  - csoler
  - G10h4ck
name: "Improve the Retroshare Android client"
requirements:
  - "Android Development Toolchain"
  - "Javascript"
  - "UI design skills"
tags:
  - GSoC2022
  - Android
---

Thanks to an automatically generated JSON API, it is now possible to interact with a running headless
Retroshare node using http requests. A Android client for retroshare core has been designed already and
very recently a user interface has been designed to work with it.

* Resolve Retroshare service Background compatibility issue. Retroshare service runs in the background and due to some restrictions of Android which currently causes the RetroShare service to stop receiving HTTP requests
* Introduce the Forum support in the retroshare mobile app as we already have in retroshare Desktop version.
* Write tests for the Whole App.
* Introduce the support of  CI/CD / Github actions.
* Provide a proper APK packaging pipeline.

Most of the machinery that allows the Android client to talk to the running Retroshare core is now 
well established, and the work in this project will consist into creating the missing functionalities
described above.

Depending on how much work is scheduled this project stands for half-time or full-time.

#### Milestones

This project requires the following steps:
* properly understanding how Retroshare JSON API works and how other clients (such as the web interface) talk to it;
* setting up the Android development environment to properly work with the existing Retroshare API
* implementing the above contributions in the form of multiple pull requests that will be merged in the project.

##### PREPARATION/BONDING

We will only recruit applicants who made proper pull requests to https://github.com/RetroShare/retroshare-mobile
before the 
selection process begins. The developer team can (and probably should) be contacted in order to get some ideas of simple contributions
to make at this step.

