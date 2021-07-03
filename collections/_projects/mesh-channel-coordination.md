---
name: "Mesh channel coordination"
desc: "Automatically select channels in mesh networks"
requirements:
 - "C programming skills"
 - "Experienced Linux knowledge (usage and architecture)"
 - "WLAN technology"
 - "Game theory"
 - "Graph theory"
difficulty: "high"

mentors:
 - "Vincent Wiemann (CodeFetch)"
initiatives:
 - GSoC
 - ffh
 - freifunk
tags:
 - OpenWrt
 - WLAN
 - Networking
 - Mesh technology
 - Game theory
 - Graph theory
 - Linux
 - C
 - Lua
collaborating_projects:
 - "freifunk"
 - "ffh Freifunk Hannover"
---

The aim of this project is to improve the quality of the wireless user
experience in mesh networks and to increase the stability of wireless mesh links
in general specifically mitigating the hidden node problem by utilizing
diverse channels where adjacent networks might otherwise interfere.

At the moment most mesh solutions define a default channel value for their
wireless mesh networks. In many cases the nodes have additional means to connect
to their neighboring nodes like direct wired connections or VPN connections.
Some nodes utilize multiple radios to reduce the hidden node problem with
diversity routing.

Upcoming features like MCCA, BSS coloring and dedicated RUs will further allow
reducing contention caused by interference.
These also need a form of coordination which has been subject of current
research and which is partly being defined in the WiFi 7 standard.

As a mesh network is a highly dynamic system and as the radio is often used to
both serve the clients and forward mesh traffic in parallel (so-called VIFs -
virtual interfaces), the configuration of the channels must be done respecting
the special properties of mesh protocols while taking route switches into
consideration and reacting accordingly. Care must be taken to not influence the
routing decisions of the mesh protocol in a way that leads to an imbalance.

An example for an imbalance occurs in dense high-use scenarios with packet-
loss-metric based mesh routing protocols if a wireless link appears to be
saturated due to interference caused by neighboring nodes and their clients.
If a redundant route exists in that case, nodes might choose another route with
a presumably better metric.
In theory that switch was assumed to be transparent to the user, but in practice
a mediocre link is often swapped for a link that e.g. has even less capacity
congesting the link long enough for some clients to assume a broken connection
and switch to another node which will eventually suffer, too.
This problem can be mitigated using adjacent channels where coverage overlaps
and a redundant connection exists.

Even though modern mesh routing protocols are hardened against some of these
issues by not only considering the packet loss for their metric calculation but
also other criteria like calculating the route metrics from wireless statistics
exported from the kernels mac80211 subsystem, they are still an open topic of
research.

For example the highly sophisticated diversity routing RFC amendment of the more
and more popular routing protocol Babel does not consider shared usage of the
radios' mesh network with the client network which can lead to unexpected
behavior as different WLAN clients tend to prefer quite individual frequencies
depending on their hardware, antenna and software configuration which could
favor an imbalance.

As this project involves a lot of different disciplines the main goal of the
student is not to get deep knowledge about every internal. Instead, the student
shall be encouraged to think and act independently then cooperatively and to
find a simple, creative way to improve the current situation.

This reflects the results-oriented approach to work which is often required for
participating in open-source projects where code changes must be kept simple to
be reviewed timely and to increase the chance of being accepted.


#### Ideas
* Create "hearing maps"
* Find ways to create hierarchical sub-trees in the network by identifying
  "border nodes" (e.g. VPN or PtP links) which is critical for distributing
  the coordination
* Only use the links which are actually needed: If a node can reach all of
  its  neighbors by other means (e.g. VPN) it should not be bound to a specific
  channel assuming the available bandwidth offered by the alternative link and
  the metric is sufficient. It may even be possible to deactivate the wireless
  mesh network for that radio to save airtime (e.g. if there is no neighbor).
  This needs to dynamically react if e.g. a new neighbor appears.
* Analyze the roaming behavior of the clients to estimate where interference
  due to the hidden node problem is more likely.
* Take actual traffic flow patterns into account.
* Identify e.g. long-range interference using coordinates if given similar
  to the WiFi 6 proposed Automatic Frequency Coordination scheme.
* Make use of game theory to achieve a Nash equilibrium instead of central
  coordination.
* Where a form of centralization is unavoidable, make the consensus fault-proof.
  The system must reconstitute timely if the elected coordinator fails.
  The Raft consensus protocol is an interesting candidate for this.
* Allow manual override

#### Milestones
* Add basic support for mesh networks in DAWN
* Implement a daemon "meshrealmd" which can interact with DAWN and implements
  the graph theory-based approach presented in the paper "Interference-Aware
  Channel Assignment in Wireless Mesh Networks" in a decentralized way
* freifunk-gluon integration (OpenWrt-based mesh framework)

#### Inspirationals
 * https://blog.freifunk.net/2018/05/19/dawn-a-decentralized-wifi-controller/
 * https://link.springer.com/chapter/10.1007/978-3-540-89183-3_7
 * https://dblp.org/pid/175/1661.html
 * https://ieeexplore.ieee.org/document/7947787/
 * https://link.springer.com/article/10.1007/s11277-019-06214-3
 * https://github.com/willemt/ticketd
 * https://en.wikipedia.org/wiki/Braess%27s_paradox
