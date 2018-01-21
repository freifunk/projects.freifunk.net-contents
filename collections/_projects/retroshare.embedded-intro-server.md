---
collaborating_projects:
  - retroshare
desc: "Create an embedded friend server inside Tor-only version of Retroshare"
developers_involved: []
difficulty: medium
status: open
initiatives:
  - GSoC
issues:
markdown: retroshare.embedded-friend-server.md
mentors:
  - csoler
name: "Embedded Tor Retroshare friend server"
requirements:
  - "Analyzing and coding"
  - "C++"
  - "Tor hidden services"
  - "http protocol"
tags:
  - C++
  - Networking
---

Retroshare is now optionally available in a Tor-only version, where the whole software runs its own Tor service, creates
its own hidden node and auto-configures it. Because hidden Retroshare nodes are totally anonymous w.r.t. their friend
nodes, it is safe to allow the software to suggest random peers to connect to.

The goal of the project is to create an embedded friend-server inside the Tor only version of RS, which will
optionnaly allow the user to publish his/her certificate and retrieve certificates of existing users, in order to make friends,
so as to bootstrap the software usage and increase its ease of adoption.

The friend server will be a .onion website, that runs pretty much like a key server, with 3 layers: (1) a single .onion meta server
which address is hard-coded in the software will list available friend servers, signed by the maintainers of the project.
(2) Friend servers will be ran independently as .onion servers, and accept/deliver keys to make friend to and (3) the GUI talks
to friend servers, receives notifications for possible new friends and allows the user to connect to them.

If enabled, Retroshare will retrieve and authenticate the servers' list using a hard-coded PGP key. Then it will post the
user's key to one of the servers and request a list of most recently published keys to make friend with.

#### Milestones

This requires the following steps:
* define the protocol to push/retrieve RS certificates to a friend server
* implement in RS the retrieval, authentication of server's list
* implement in RS the publication and retrieval of keys from a friend server
* implement the web service that accepts/delivers certificates
* add in GUI a good looking friend suggestion system based on what's found on the friend servers

##### PREPARATION/BONDING

* understand how RS certificates works
* get a reasonnably good understanding of the structure of the project
* discuss possible protocols and options with the developers

