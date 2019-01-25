---
name: "BMX7 WireGuard for tunnels"
desc: "Etablish encrypted tunnels between devices via WireGuard"
requirements:
  - "c"
  - "bmx7"
  - "wireguard"
difficulty: hard
issues:
  - ""
mentors:
  - axn
  - aparcar
initiatives:
  - GSoC
tags:
  - wireguard
  - crypto
  - GSoC2019
  - web
  - mesh
  - bmx6
  - bmx7
collaborating_projects:
  - libremesh
  - freifunk
status: open
---

The routing protocol BMX7 offers a great way to extend it's functionally via
[plugins][0]. They're used for the distribution of small files, settings up
tunnels or offer stats of the network structure.

Currently the connection between a client node and the gateway are established
via IPIP, which is unencrypted and therefore possibly readable by attackers. As
mesh networks usually operate on unencrypted wireless connections, the attack
vector is considerably big.

A possible solution would be to combine the current cryptographic stack of BMX7
with the one used by WireGuard. It would be possible to replace the current keys
of BMX7 the ones used by WireGuard and thereby allow not only signing of
[descriptive updates][1], but also encrypt traffic if desired.

As an alternative to lower the difficulty from hard to medium, it would be
possible to simply announce public WireGuard keys additionally and *only* create
a new tunnel plugin.

#### Milestones

* Understand BMX7 functionality and description system
* Understand the BMX7 plugin system
* Understand the cryptography used by BMX7 and WireGuard
* Replace BMX7 private/public keys with compatible WireGuard ones.
* Add a plugin to etablish encrypted connections, replacing the current
  [tunnel][2] plugin.

[0]: https://github.com/bmx-routing/bmx7#bmx7-plugins
[1]: https://github.com/bmx-routing/bmx7#descriptions
[2]: https://github.com/bmx-routing/bmx7/tree/master/lib/bmx7_tun

##### PREPARATION/BONDING

* Install a minimal bmx7 setup for testing
* Join the [BMX7 matrix chat][2]
