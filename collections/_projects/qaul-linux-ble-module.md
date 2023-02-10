---
name: "qaul BLE Module for Linux with BlueR"
desc: "Create a Linux BLE (Bluetooth Low Energy) module which compatible to the two existing modules for Android & iOS."
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
issues: https://github.com/qaul/qaul.net/issues/314
markdown: qaul-linux-ble-module.md
mentors:
  - MathJud
requirements:
  - "Rust"
  - BLE
tags:
  - GSoC2023
  - qaul
  - Rust
  - Bluetooth
  - BLE
  - peer2peer
  - libp2p
---

# qaul BLE Module for Linux with BlueR

**Create a BLE (Bluetooth Low Energy) module in rust which compatible to the two existing modules for Android & iOS.**

Create a BLE (Bluetooth Low Energy) module in rust which compatible to the two existing modules for Android & iOS.

Existing android BLE module:
<https://github.com/qaul/qaul.net/tree/main/android/blemodule>

It shall do the following things:

* Listen for BLE advertisements
  * detect neighbour nodes
* Send BLE advertisement messages in regular intervals.
* send arbitrary binary data to nodes nearby.
* receive arbitrary binary data from nodes nearby.

The module is independent and will communicate via protobuf to the controlling backend library libqaul.

`BlueR` is the official Bluetooth low energy repository for for rust.
<https://github.com/bluez/bluer>

Prototypes with partial functionality already exist.

## About qaul

[qaul](https://qaul.net) is an Internet independent wireless mesh communication app. To communicate P2P directly from device to device and mesh all interconnected devices together.
qaul.net interconnects Android, iOS, Linux, MacOS & Windows devices via LAN, Bluetooth and Internet overlay connections.

qaul is written in rust, uses rust-libp2p internally and has a cross platform flutter GUI.

<https://qaul.net>

## Resources

* [qaul github repository](https://github.com/qaul/qaul.net)
* [BlueR Rust BLE library](https://github.com/bluez/bluer)

## Milestones

* setup rust protobuf communication with libqaul
* create advertising (prototype exists)
* create scanning (prototype exists)
* create GATT service for ID exchange
* send message
* receive message

## Applying for this Project

Please get in contact with the Mentor @MathJud (via [Email](mailto:jud@qaul.net) or [qaul matrix chat #qaul.net:c-base.org](https://matrix.to/#/#qaul.net:c-base.org)) to discuss and prepare your application and project.
