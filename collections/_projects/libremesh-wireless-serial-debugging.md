---
name: LibreMesh Wireless Serial Console Access
desc: Develop software and hardware to securely access routers serial console wirelessly
maskdown: libremesh-wireless-serial-debugging.md
collaborating_projects:
  - libremesh
  - altermundi
developers_involved: []
difficulty: medium
status: open
initiatives:
  - GSoC
issues:
mentors:
  - ayalaluquez
  - G10h4ck
requirements:
  - "Lua programming language"
  - "Networking knowledge"
  - "Basic electronic knowledge"
  - "Hardware for testing"
tags:
  - GSoC
  - OpenWrt
  - LibreMesh
  - Networking
  - Community Networks
  - LORA
  - ESP
  - Hardware
---

In community networks it is a common issue that a router is not reacheable
remotely with causes ranging from misconfiguration to hardware failure.
In addition, it might be difficult to physically access the router because of
where it is installed, often on top of high poles. Some time one have to climb
on a tower just because by error the networking stack has been disabled, or to
discover the device is burned and need hardware replacement.
Most routers have UART serial port on-board, which might be last resort
debugging companinion in those cases, but it is unaccessible unless you climb
the tower, open the router solder some pin etc.
Having the possibility to access the serial console wirelessly in those cases
would be a bonanza in such cases.
This GSoC proposal is aimed to give secure wireless serial console access to the
router.

A possible solution could involve the usage of a ESP8266 connected to the router
UART port, broadcasting a password protected WiFi.
Another possible way to solve this could involve some LORA enabled device
connected to the router UART port.


#### Milestones

##### GSoC Community Bonding

* The student aquire basic electronic devices to work on the project.
* The student must learn how to contribute code via merge request mechanism.
* The student should relate comfortably with the LibreMesh developers.
* The student should individuate one or more real world comminity network and establish a fluid cooperation relationship with them.


##### GSOC Midterm

* A cheap hardware module to associate to routers to enable secure wireless serial console access.
* Software to take advantage of this solution should be ready to be tested on community networks.


##### GSOC Final

* Deployment of the solution in all the nodes of the chosen community network.
