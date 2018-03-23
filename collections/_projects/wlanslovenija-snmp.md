---
name: "nodewatcher: SNMP support for monitoring"
desc: "Implement SNMP support for monitoring in nodewathcer."
requirements:
 - "Python/Django, SNMP experience."
difficulty: "medium"
mentors:
 - kostko
initiatives:
 - GSoC
tags:
 - GSoC2018
 - nodewatcher
collaborating_projects:
 - wlanslovenija
---

Currently nodewatcher uses its own HTTP-based monitoring protocol. But this requires custom firmware on the node. It would be great if nodewatcher could support devices in the network which simply publish data using SNMP.

Student should have experience or be willing to learn Python and Django and how to write Django apps together with basic understanding of HTML/JavaScript and general web development. Understanding of SNMP is a plus.

#### Milestones

* Learn about the nodewatcher and its monitoring system.
* Deploy a test network locally to see monitoring system in action using Docker.
* Add to your test network a simple SNMP node.
* Implement SNMP monitoing in nodewatcher, mapping values to nodewatcher monitoring schema.
* Make sure SNMP implementation works with popular WiFi devices, like UniFi APs.
* Document and implements tests.
