---
name: "qaul RPC user authentication layer"
desc: "libqaul <-> GUI protobuf RPC authentication"
collaborating_projects:
  - qaul
developers_involved:
  - MathJud
difficulty: medium
size: "350 hours"
status: open
initiatives:
  - GSoC
  - GSoC2023
issues: https://github.com/qaul/qaul.net/issues/531
markdown: qaul-user-authentication.md
mentors:
  - MathJud
requirements:
  - "Rust"
  - Protobuf
tags:
  - GSoC2023
  - qaul
  - Rust
  - libp2p
  - "Noise Protocol"
  - Cryptography
  - Authentication
---

# User Authentication Layer

The GUI communicates via protobuf RPC messaging with libqaul. At the moment there is only one user per node. libqaul is capable of having multi users per node. The GUI <-> libqaul RPC communication shall be organized in sessions. Each session shall be authenticated and encrypted.

The user authentication layer shall have the following qualities:

* Secure authentication mechanism
  * optional user password.
* The system should be zero-config for the user. A password and/or a session key (which can be cached) can be used.
* The system shall support multiple sessions per user & multiple users per node.
* Each session shall be transport encrypted via the Noise protocol.

This work is also the foundation of a possible web interface in qaul, in which users interact with a node via a web GUI.

## Milestones

* During application period: Create a concept for your project. Discuss your concept with a mentor.
  * Define the authentication system
  * Define the encryption system
* Define the Protobuf communication structure
* Implement the Sessions.
  * Implement the sessions into the CLI application.
* Implement the Authentication system.
* Encrypt the sessions

## Resources

* [qaul Protobuf RPC](https://github.com/qaul/qaul.net/tree/main/rust/libqaul/src/rpc)

## About qaul

[qaul](https://qaul.net) is an Internet independent wireless mesh communication app. To communicate P2P directly from device to device and mesh all interconnected devices together.
qaul.net interconnects Android, iOS, Linux, MacOS & Windows devices via LAN, Bluetooth and Internet overlay connections.

qaul is written in rust, uses rust-libp2p internally and has a cross platform flutter GUI.

<https://qaul.net>

## Applying for this Project

Please get in contact with the Mentor @MathJud (via [Email](mailto:jud@qaul.net) or [qaul matrix chat #qaul.net:c-base.org](https://matrix.to/#/#qaul.net:c-base.org)) to discuss and prepare your application and project.
