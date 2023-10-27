---
name: "qaul Matrix Bridge"
desc: "Create a matrix bridge for the qaul messenger App"
collaborating_projects:
  - qaul
developers_involved:
  - MathJud
  - Saces
difficulty: medium
size: "350 hours"
status: completed
initiatives:
  - GSoC
  - GSoC2023
issues: https://github.com/qaul/qaul.net/issues/530
markdown: qaul-matrix-bridge.md
mentors:
  - MathJud
  - saces
requirements:
  - "Rust"
  - Go
  - Protobuf
tags:
  - GSoC2023
  - qaul
  - Rust
  - Go
  - Matrix
  - Protobuf
---

# qaul <-> Matrix Bridge

Write a matrix bridge for qaul, to be able to interconnect qaul with matrix and all supported communication protocols by matrix. This shall allow to send qaul messages to matrix, signal messenger, WhatsApp, Telegram, etc.

A matrix bridge is interconnects matrix with other systems. There are already matrix bridges for many other messengers (Signal messenger, WhatsApp, Telegram, etc.). With the qaul-matrix bridge we could interconnect qaul to all these messengers.

The bridge shall have the following qualities:

1) **Relay Bridge**: creates a relay bot for matrix & qaul
2) **Double-Puppeting**: makes users from one system appear as users in the other system.

This project can be split into different parts.

## About qaul

[qaul](https://qaul.net) is an Internet independent wireless mesh communication app. To communicate P2P directly from device to device and mesh all interconnected devices together.
qaul.net interconnects Android, iOS, Linux, MacOS & Windows devices via LAN, Bluetooth and Internet overlay connections.

qaul is written in rust, uses rust-libp2p internally and has a cross platform flutter GUI.

<https://qaul.net>

## Resources

* [Matrix bridge documentation](https://matrix.org/bridges/)
* Libqaul communication services
  * [Public messaging](https://github.com/qaul/qaul.net/tree/main/rust/libqaul/src/services/feed)
  * [Chat messaging](https://github.com/qaul/qaul.net/tree/main/rust/libqaul/src/services/chat)
  * [qaul users](https://github.com/qaul/qaul.net/blob/main/rust/libqaul/src/node/user_accounts.rs)

## Milestones

* create a concept for your project (application phase)
* create a detailed concept for the relay bridge
* implement the relay bridge
  * implement the libqaul part in rust
  * create a golang matrix communication part
* create a detailed concept for double-puppeting
* implement the double-puppeting, as far as defined
  * implement the libqaul part in rust
  * create a golang matrix communication part

## Applying for this Project

Please get in contact with the Mentor @MathJud (via [Email](mailto:jud@qaul.net) or [qaul matrix chat #qaul.net:c-base.org](https://matrix.to/#/#qaul.net:c-base.org)) to discuss and prepare your application and project.
