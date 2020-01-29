---
name: "RetroShare OpenDHT integration"
desc: "Write a RetroShare discovery service based on OpenDHT"
markdown: retroshare-opendht.md
collaborating_projects:
  - RetroShare
  - OpenDHT
developers_involved:
  - aberaud
  - AmarOk1412
difficulty: medium
status: open
initiatives:
  - GSoC
issues:
  - https://github.com/savoirfairelinux/opendht/issues/399
  - https://github.com/savoirfairelinux/opendht/issues/398
mentors:
  - csoler
  - G10h4ck
requirements:
  - "Analyzing and coding"
tags:
  - GSoC
  - C++
  - DHT
---


As of today RetroShare has it's own implementation of bittorrent DHT called
libbitdht, it's code is quite old and when some bug has arised it have been
difficult to dig into it. When RetroShare added support for DHT writing our own
library was the best option available but since then the word has changed a lot.
Nowadays OpenDHT library is available and implement almost all we need to
substitute libbitdht.
This project aim to create a retroshare module based on OpenDHT that could
substitute libbitdht, first of al a couple of missing feature should be
implemented in OpenDHT, and then a RetroShare service sto wrap around OpenDHT
should be implemented.
At moment libbitdht and OpenDHT should be able to coexist, but in the long run
we might decide to drop libbitdht completely.


#### Milestones

##### GSoC Community Bonding

* Get familiar with the RetroShare network
* Get familiar with the RetroShare code
* Get familiar with the OpenDHT code
* Discuss possible developments options with the developers


##### GSOC Midterm

* Solve https://github.com/savoirfairelinux/opendht/issues/399
* Solve https://github.com/savoirfairelinux/opendht/issues/398
* Basic implementetion of a RetroShare service that integrate OpenDHT into RetroShare
* To be defined by candidate proposal


##### GSOC Final

* To be defined by candidate proposal
