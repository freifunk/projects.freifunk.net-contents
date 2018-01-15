---
collaborating_projects:
  - retroshare
desc: "Create a Wall/Blog system based on GXS in Retroshare"
developers_involved: []
difficulty: medium
status: open
initiatives:
  - GSoC
issues:
markdown: retroshare.wall-plugin.md
mentors:
  - Cyril Soler
name: "Create a social network plugin based on GXS"
requirements:
  - "Analyzing and coding"
  - "C++"
  - "GXS"
tags:
  - C++
  - Decentralized social network
---

Retroshare contains a generic distributed database system (called GXS) which allows to share data between nodes, 
in a way that is cryptographically secured (database access may be limited to circles of people, etc). This database 
system is currently used for distributing forums and channels over the network. The GXS system also offers 
the possibility to respond, submit comments, and vote over posts. 

We would like to use it to create a service that 
allows users to create a blog-like service, to which friend nodes subscribe so as to propagate the info over the 
network. Depending on the student's skills and motivation, such a plugin could offer one of the following similar 
services: twitter (distributed micro-blogging), blog (distributed blogging), Wall (facebook style information sharing).

This is not an easy project, since GXS internals are hard to understand in the first place. But the devs are highly motivated to get it done.

#### Milestones

* properly represent social network objects (posts,images,comments,...) using internal GXS primitives (Groups, Circles, Identities, etc). This is to be discussed with the developers.
* create the plugin interface to the backend. 
* create the GUI for the Wall/Twitter/Blog service (preferably Qt. Could be Json+web, but would add some complexity)
* implement the backend service, based on GXS interaction handles

##### PREPARATION/BONDING

* get familiar with the Retroshare network 
* understand how GXS works. A white paper is available here: https://hal.inria.fr/hal-01617423 
* discuss possible options with the developers

