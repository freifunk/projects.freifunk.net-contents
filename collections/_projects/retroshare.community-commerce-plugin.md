---
collaborating_projects:
  - retroshare
desc: "RetroShare Create a local community commerce discovery plugin"
developers_involved: []
difficulty: medium
status: open
initiatives:
  - GSoC
issues:
markdown: retroshare.community-commerce-plugin.md
mentors:
  - csoler
  - G10H4ck
name: "RetroShare Create a local community commerce discovery plugin"
requirements:
  - "Analyzing and coding"
  - "C++"
  - "GXS"
tags:
  - C++
  - Decentralized market
  - GSoC2019
---

Retroshare contains a generic distributed database system (called GXS) which
allows to share data between nodes, in a way that is cryptographically secured
(database access may be limited to circles of people, etc).
This database system is currently used for distributing forums and channels over
the network. The GXS system also offers the possibility to respond, submit
comments, and vote over posts.

We would like to use it to create a service that allows users to create a
decentralized local community market service, to which friend nodes subscribe so
as to propagate the info over the network, which include merketed products and
customers reviews.
The key concept is that a seller whith good reputation from friends is much more
trustworty then a seller with review from unkown people.

This is not an easy project, since GXS internals are hard to understand in the
first place. But the devs are highly motivated to get it done.

#### Milestones

* properly represent social network objects (posts,images,comments,...) using internal GXS primitives (Groups, Circles, Identities, etc). This is to be discussed with the developers.
* create the plugin interface to the backend. 
* create the GUI for the Wall/Twitter/Blog service (preferably Qt. Could be Json+web, but would add some complexity)
* implement the backend service, based on GXS interaction handles

##### PREPARATION/BONDING

* get familiar with the Retroshare network 
* understand how GXS works. A white paper is available here: https://hal.inria.fr/hal-01617423 
* discuss possible options with the developers

