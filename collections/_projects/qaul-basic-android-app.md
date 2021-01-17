---
name: "qaul basic Android app"
desc: "Create a basic qaul android app"
collaborating_projects:
  - qaul
developers_involved: []
difficulty: medium
status: open
initiatives:
  - GSoC
issues: https://git.qaul.org/qaul/qaul/-/issues/1
markdown: qaul-basic-android-app.md
mentors:
  - spacekookie
requirements:
  - "Android"
  - "Rust FFI"
  - "Kotlin"
  - "Java"
tags:
  - GSoC2021
  - qaul
  - Android
---

`qaul.net` is an ad-hoc wireless mesh networking app, and development
framework created in 2011 and used by various activists and projects
around the world.  Its aim is to make it easier to bring internet/
network access to places that currently don't have any, and to connect
participants in a network together directly when no other
infrastructure is available.

Since 2019 the project has been undergoing a complete re-write in Rust
in order to support modern mobile hardware, and provide a more
flexible architecture that other developers can use to write
applications on-top of.

We are searching for students who want to participate in this
re-write, with the goal of becoming long-term contributors to the
project.

The qaul application architecture uses an RPC protocol to connect
client to a persistant server that handles user, message, and network
abstractions.  In order to access these from Android code, some
bindings in Java (or Kotlin) need to be created

The scope of this project is to take the existing Android application
code and update it to modern Android best-practises.  There are
several screens that need to be designed, and ideally would use
re-usable mechanisms to be extensible in the future.

The main functionality of the app would be to bind against the basic
qaul RPC functions to allow creation, login, and deletion of user
identities, as well as sending simple chat messages to other
participants on the network.

Using peer-to-peer networking mechanisms (WifiDirect, Bluetooth LE,
Wifi Aware, ...) is not in-scope for this project!


#### Milestones

* Modernise/ update the code base to best practises
  * This can include using external libraries to manage application/ view states
* Create bindings to the core functions of the qaul RPC libraries
* Launch the qaul backend service and connect to it via the RPC bindings
  * Create/ delete users, manage user metadata (username, avatar, etc)
* Implement a very basic chat view, using the qaul-chat service


##### PREPARATION/BONDING

* Gain a general understanding of how the qaul architecture works
* Study the qaul RPC layer and application development flow
* Study the existing Android app code
* Discuss possible development with mentors
