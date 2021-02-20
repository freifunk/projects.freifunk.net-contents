---
name: "RetroShare Web Interface"
desc: "Continue the development of the Web interface based on the JSON API of Retroshare"
markdown: retroshare-webui.md
collaborating_projects:
  - RetroShare
developers_involved:
  - csoler
  - G10H4ck
  - saud
difficulty: easy
status: open
initiatives:
  - GSoC
  - GSoC2021
mentors:
  - csoler
  - G10h4ck
requirements:
  - "JSON, Javascript"
tags:
  - GSoC
  - GSoC2021
  - Javascript
  - Web interface
---

During 2019 GSoC session, the framework for the Web interface of retroshare was first initiated and developed.
The  Web interface is made in Javascript and uses Retroshare automated JSON API interface to communicate with the
internals of libretroshare. It already has its own building system and already works, although it is rather incomplete.

The work in this project consists in developing the remaining Javascript code to complete the Web interface, which
includes the configuration panel, the access to channels, forums and boards, as well as the handlign of GXS identities.
A plus would also be to add a pannel for statistics, showing various aspects of the internal variables of file transfer,
GXS synchronisation, so that the software can easily be run on a headless server.

Although this project is fairly easy, it requires some reasonnable knowledge of JS. The project do not aim to changing
the current framework the Web interface is based on, nor its internal algorithmics. There is no specific order in which the
different aspects of the Web interface can be covered by the candidate. A proof of involvement (a few commits fixing
simple issues) will be requested in order to select motivated applicants.

#### Milestones

##### GSoC Community Bonding

* Get familiar with the RetroShare network, and contact the main developers.
* Get familiar with the existing Web interface code
* Discuss possible developments options with the developers

##### GSOC Midterm

* To be defined by candidate proposal

##### GSOC Final

* To be defined by candidate proposal
