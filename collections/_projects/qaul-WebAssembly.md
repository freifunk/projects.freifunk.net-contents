---
name: "qaul WebAssembly Client"
desc: "Create a progressive web app client for qaul"
collaborating_projects:
  - qaul.net
  - qaul
developers_involved: []
difficulty: advanced
size: full-time
status: open
initiatives:
  - GSoC
  - GSoC2022
issues: https://github.com/qaul/qaul.net/issues/315
markdown: qaul-WebAssembly.md
mentors:
  - MathJud
requirements:
  - "Rust"
  - WebAssembly
tags:
  - GSoC2022
  - qaul
  - Rust
  - WebAssembly
  - Wasm
  - peer2peer
  - libp2p
  - flutter
  - protobuf
---

# WebAssembly Client for qaul

**Create a progressive web app client for qaul**

With WebAssembly one can load compiled code as a progressive web app into a web browser. 
New API's such as WebBluetooth can be used to interconnect with other devices directly from within the web browser.

The scope of this project is to compile libqaul and the underlying rust-libp2p for webassembly and find solutions for problematic modules.

The underlying library rust-libp2p compiles to WASM, and also the used database is WASM compatible.
It will be interesting to test with the connection modules what will be possible in relation to network transports.

To have storage and cryptography within the browser is the main part of the project and crucial for secure decentralized p2p networks.


## About qaul

`qaul.net` is an Internet independent wireless mesh communication app . 
qaul.net interconnects Android, iOS, Linux, MacOS & Windows devices via LAN, Bluetooth and Internet overlay.

qaul is written in rust, uses rust-libp2p internally and has a cross platform flutter GUI, all communication is protobuf encoded and encrypted.

https://qaul.net


#### Resources

* [qaul github repository](https://github.com/qaul/qaul.net)
  * [libqaul rust library](https://github.com/qaul/qaul.net/tree/main/rust/libqaul)
  * [rust-libp2p](https://github.com/libp2p/rust-libp2p)
  * [sled database](https://sled.rs/)
* [flutter GUI](https://github.com/qaul/qaul.net/tree/main/qaul_ui)

#### Milestones

* Compile libqaul for WebAssembly
  * Check each module for compatibility
* Interface with flutter weg GUI
* Test & Play with the WebAssembly App & WebAssembly functionality
  * Bluetooth Module
  * MDNS module


#### PREPARATION/BONDING

Please get in touch with [Mathias](mailto:jud@qaul.net) when you're interested doing this task or another task for the prohject, he will help you develop your project.

