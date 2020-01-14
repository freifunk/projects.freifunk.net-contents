---
name: "qaul.net Location & Map Service"
desc: "Develop qaul.net Location & Map Services"
collaborating_projects:
  - qaul.net
developers_involved: []
difficulty: medium
status: open
initiatives:
  - GSoC
issues: https://git.open-communication.net/qaul/qaul.net/issues/121
markdown: qaul.net_Location-Service.md
mentors:
  - MathJud
  - luxferresum
  - spacekookie
requirements:
  - "HTML CSS Javascript"
  - "EmberJS"
  - "Frontend Affinity"
tags:
  - GSoC2020
  - qaul.net
  - GUI
  - Web Technology
---

`qaul.net` is a mesh networking communication app that has been around since 2011
with active users around the world, using it instead of traditional internet
infrastructure to share files, data and communicate.

The project is now undergoing a complete re-write in Rust in order to support
more modern hardware, be more maintainable and extendable. The HTML5 GUI is rewritten
in EmberJS framework. 

The rewrite is in it's alpha state and will become beta during the GSoC project.
We are searching for students who want to be a part of this rewrite, with the idea to become longer term contributers to the project.

A new feature for the qaul.net application is to have the possibility for a user to send their location to other people in the network and to map and share local points of interests on a limited locally available (offline) map.

A person working on this task would be responsible for the creation of a user interaction concept and it's implementation in with `EmberJS` framework in the user interface. 
A conceptually tricky part will be the concept for 'offline' maps within the location service.

To have an "offline" location service that can not only send the users location 
information but also geographically localize points of interests - from police 
violence in demonstrations to people in need during desaster recovery - will 
be a vital and critical part of the qaul.net application.


#### Milestones

* Develop user experience & technical concept
  * What are the interaction possibilities?
  * How will it look and feel like?
  * How is diplaying a map in a situation without internet access possible?
    * What could be intelligent strategies?
  * What map format could be chosen?
  * What is the data that needs to be exchanged and how can it be handled in a decentralized manner.
* Implement the technical concept
  * implement the location sharing
  * implement the mapping technique
* Finish the UI implementation'
  * Test the user experience


##### PREPARATION/BONDING

* Get a general understanding of how qaul.net works
* Get a general understanding of `EmberJS` base HTML5 GUI
* Learn mapping techniques
* Discuss possible development with mentors
