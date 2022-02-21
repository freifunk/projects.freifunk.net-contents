---
name: "Mesh beacons: low bitrate communication in disconnected mesh radios"
desc: "Provide a mechanism for mesh nodes to exchange (more) information with their peers without the need to be associated (scanning only). This has many usefull use cases, from knowing the name of the node before connecting, to aiding antenna alignment with low quality signal, etc."
requirements:
 - "The applicant needs to have an understanding of low level programming."
difficulty: medium
size: "full-time"
status: open
issues:
 - "https://github.com/libremesh/lime-packages/issues/875"
mentors:
 - spiccinini
 - gferrero
initiatives:
 - GSoC
 - GSoC2022
requirements:
 - "C programming language"
tags:
 - LibreMesh
 - 802.11s
 - OpenWrt
 - Linux kernel
collaborating_projects:
 - libremesh
 - altermundi
---

Exchanging information between disconnected 802.11s peers is important because connection takes a lot of time and/or the signal quality is not enough to reliably connect but is enough to send/receive some packets.
In OpenWrt 802.11s implementation there is no known easy way to add and retrieve information in the beacons albeit the specification of 802.11s provides ways of adding custom information. 
The student will have to study the Linux kernel implementation of 802.11s to double check if Linux provides a way to add information to the baeacons and also a way to retrieve this custom information.

If there is no support in Linux then the project can take two paths:

1. develop and try to upstream 802.11s beacons customization to the Linux kernel.
2. investigate current solutions to exchange information in disconnected radios (for example using packet injection/sniffing on monitor interfaces), and try to develop a prototype solution.


#### Milestones

##### GSOC 2022 COMMUNITY BONDING

* Conceptual work should produce a coherent proposal to be submitted to the community for the review.
* The applicant should have joined all of the communication channel of the project and met the community in the periodic online meetings.
* An initial blog post will be written, with the invitation to propose alternative solutions for the identified challenges.

##### GSOC 2022 MIDTERM

* Conceptual work should be completed, the functions to be implemented and the tools should be fixed.
* The applicant should have a working testing platform, either physical or virtual.
* A mid term blog post will be written.

##### GSOC 2022 FINAL

* Everything has to be reviewed and merged.
* Documentation should be available.
* A final blog post will be written.
