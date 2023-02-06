---
name: "Implement traffic priorization in Pirania captive portal for mesh networks"
desc: "Pirania captive portal is a voucher-based captive portal used in LibreMesh. In order to have guest access, this should have a lower priority, managed via Traffic Control."
requirements:
 - "The applicant needs to have understanding of networking in mesh networks."
difficulty: "high"
size: "350 hours"
issues:
 - "https://github.com/libremesh/lime-packages/issues/261"
 - "https://github.com/libremesh/lime-packages/issues/244"
mentors:
 - spiccinini
 - Ilario
initiatives:
 - GSoC
 - GSoC2023
tags:
 - LibreMesg
 - Pirania
 - TC
 - SQM
collaborating_projects:
 - libremesh
 - altermundi
---

Pirania captive portal is already in production in some community networks running LibreMesh on their routers.
The usage of Pirania helps the community to pay the bill from the internet service provider.
But LibreMesh project also tries to open the access to the local and remote digital resources to everyone, and for this reason the availability of a guest access would be reccomended.
This will require that the presence of a connected guest client does not slow down the connection of the owner of the gateway or of who actually paid for having a Pirania voucher.
In order to achieve this, the data packets needs to have different priorities depending on the originating client, diregard the mesh node (access point) this client is connected to.
The problem is absolutely non-trivial, and the technical tools needed will be at least Traffic Control, Smart Queue Management, and iptables.

#### Milestones

##### GSOC 2023 COMMUNITY BONDING

* Conceptual work should produce a coherent proposal to be submitted to the community for the review.
* The contributor have a fork of the lime-packages repository and have learnt the basics of Git.
* The applicant should have joined all of the communication channel of the project and met the community in the periodic online meetings.
* An initial blog post will be written, with the invitation to propose alternative solutions for the identified challenges.

##### GSOC 2023 MIDTERM

* Conceptual work should be completed, the functions to be implemented and the tools should be fixed.
* The applicant should have a working testing platform, either physical or virtual.
* The applicant should be familiarized with LibreMesh configuration and running.
* The applicant should be familiarized with Pirania configuration and running.
* The applicant should be familiarized with iptables configuration and running.
* The applicant should be familiarized with Traffic Control for Smart Queue Management configuration and running.
* A mid term blog post will be written.

##### GSOC 2023 FINAL

* The patch for Pirania should be functional even if not completely polished.
* Everything has to be reviewed and merged.
* Unit testing tests should be ready.
* Documentation should be available.
* A final blog post will be written.
