---
name: "BMX7 IPv6 distribution plugin"
desc: "Distribute public IPv6 addresses from a gateway to clients"
requirements:
  - "bmx7"
  - "IPv6"
  - "c"
difficulty: medium
issues:
  - ""
mentors:
  - axn
  - aparcar
initiatives:
  - GSoC
tags:
  - ipv6
  - GSoC2019
  - web
  - mesh
  - bmx6
  - bmx7
collaborating_projects:
  - libremesh
  - freifunk
status: in_review
---

The routing protocol BMX7 offers a great way to extend it's functionally via
[plugins][0]. They're used for the distribution of small files, settings up
tunnels or offer stats of the network structure.

BMX7 uses it's own IPv6 addresses to communicate within the mesh, however, for
now it is not possible to assign public IPv6 subnets of a gateway to other
nodes. While this is manually possible, an automatic solution is missing.

Goal is to enable IPv6 on client nodes, make them as a gateway for a subnet and
once granted, offer IPv6 addresses to clients (Smartphones, Computers) of the node.

The gateway tracks distributed IPv6 subnets similar to a DHCP server. Client
nodes may also request a subnet again, where the gateway node can decide based
on previous distribution if the request is granted. This is possible by linking
the [BMX7 global ID][1] with IPv6 subnets.

[0]: https://github.com/bmx-routing/bmx7#bmx7-plugins
[1]: https://github.com/bmx-routing/bmx7#global-id

#### Milestones

* Understand BMX7 functionality and routing concept
* Understand the BMX7 plugin system
* Create a plugin for gateway nodes, offering subnets and track distribution
* Create a plugin for client nodes, requesting at gateway nodes subnets of
  specific sizes

##### PREPARATION/BONDING

* Install a minimal bmx7 setup for testing
* Join the [BMX7 matrix chat][2]

[2]: https://riot.im/app/#/room/#bmx-routing:matrix.org
