---
name: "qaul.net WebAssembly Prototype"
desc: "Create a progressive web app prototype for qaul.net"
collaborating_projects:
  - qaul.net
  - qaul
developers_involved: []
difficulty: medium
status: open
initiatives:
  - GSoC
issues: https://git.open-communication.net/qaul/qaul.net/-/issues/137
markdown: qaul-WebAssembly.md
mentors:
  - MathJud
requirements:
  - "Rust"
  - WebAssembly
tags:
  - GSoC2021
  - qaul.net
  - Rust
  - WebAssembly
  - Wasm
  - Bluetooth
  - BLE
  - peer2peer
---

# WebAssembly Prototype for qaul.net

**Create a progressive web app prototype for qaul.net**

With WebAssembly one can load compiled code as a progressive web app into a web browser. 
New API's such as WebBluetooth can be used to interconnect with other devices directly from within the web browser.

The scope of this project is to create a progressive web app prototype of qaul.net and to explore how far a progressive web app can replace native clients.

As qaul.net is written in the programming language rust which can be compiled to WebAssembly and has a webGUI, it makes it suitable to run in the web browser.


## About qaul.net

`qaul.net` is an ad-hoc wireless mesh networking app to communicate directly with other users in proximity without any Internet connectivity. 
qaul.net interconnects many operating systems and devices via Wifi, Bluetooth and local networks.
The project started in 2011 and is currently rewritten in the programming language rust.

qaul.net routes everything in user space and creates an identity based routed mesh network.

qaul.net is developed by the 'Open Community Project Association', is funded by various foundations and is looking for students who want to participate in this GSoC, with the goal of becoming long-term contributors to the
project.

https://qaul.net


#### Milestones

* Create small prototypes
  * Rust & WebGui as WebAssembly app in Browser
  * Use WebBluetooth API in WebAssembly
  * Store data in WebAssembly
* Compile qaul.net for WebAssembly
* Create working app
* Test & Play with the WebAssembly App & WebAssembly functionality


##### PREPARATION/BONDING

* Study WebAssembly
  * How to compile rust for WebAssembly
  * How to use WebBluetooth in WebAssembly
* Gain a general understanding of how the qaul architecture works
* Discuss possible development with mentors
