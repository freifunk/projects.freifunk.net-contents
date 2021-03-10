---
name: "Babeld statistics"
desc: "Adding collectd/prometheus statistic plugins for babeld"
status: in_review
requirements:
 - C
 - lua
difficulty: "middle"
mentors:
 - PolynomialDivision
initiatives:
 - GSoC
tags:
 - OpenWrt
collaborating_projects:
 - "OpenWrt upstream"
---

More and more Freifunk Communities are switching to babeld as mesh daemon. However, statistics about route-change-updates, rx-costs, rtt-times to neighbors, and other babeld related metrics are not collected. Implement for collectd/prometheus a plugin that makes those statistics available.