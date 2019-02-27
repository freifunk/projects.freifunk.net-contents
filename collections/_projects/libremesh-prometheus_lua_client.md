---
name: "LiMe prometheus-lua-client for OpenWrt"
desc: "LiMe prometheus-lua-client for OpenWrt"
difficulty: medium
status: open
initiatives:
  - GSoC
issues:
markdown: libremesh-prometheus_lua_client.md
mentors:
  - G10h4ck
  - nicopace
requirements:
  - experience programming in Lua
  - understanding of prometheus
  - basic knowledge of a community network
tags:
  - Lua
  - Prometheus
  - LibreMesh
  - OpenWrt
---

When the size of a community network grow beyond a few tens of nodes, retrieve,
store and organize network's devices healt state data over time becomes too
complex.

[Prometheus](https://prometheus.io/) is often the regarded as the most used
software to solve this kind of problems, but it lacks proper support for
embedded devices that are widely used in community networks.

Because of this, in this GSoC we propose to make a light and simple
implementation in Lua of the
[Prometheus's metrics](https://prometheus.io/docs/concepts/metric_types/)
(Counter, Gauge, Histogram and Summary) and develop the instrumentation of the
most necessary and common things to measure.


#### Milestones

* Develop the library of Prometheus metrics in lua with minimal dependencies.
* Implement Prometheus instruments we need as modules.
* Test it with a Prometheus instance.

#### Preparation/Bonding

- https://prometheus.io/docs/instrumenting/writing_clientlibs/
