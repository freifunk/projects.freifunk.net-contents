---
collaborating_projects:
  - freifunk
desc: "Extend or develop an App for Android to allow phone calls to local contacts"
developers_involved: [ ]
difficulty: high
status: open
initiatives:
  - GSoC
issues:
markdown: local_network_phone_app.md
mentors:
  - mwarning 
name: "Local Phone App"
requirements:
  - "Analyzing and coding"
  - "Programming"
  - "IPv6"
tags:
  - app
  - GSoC2018
  - android
  - qr-code
  - webrtc
---

All telephone apps work only with a central server on the Internet, which is not available by default in community networks. To be able to talk to some other contact on the local network, without the need for an Internet connection, would give community networks a more practical meaning apart from providing only Internet access. This would also be useful for communication in desaster areas.

To share a contact, at least the MAC address of the wireless interface is shared via QR-Code. The App can use the MAC address to find the communication partner on the local network. This could be accomplished e.g. via connecting to the EUI-64 IPv6 address of the local network, by using IPv6 neighborhood discovery / IPv4 ARP probing, or any other suitable method.
Working in an IPv6 only environment is required and essentially easier. IPv4 support is optional.

The audio transfer is best accomplished via WebRTC, at it is probably the easiest way to establish an audio or even a video link. If the app already has a means of audio transfer, this would be fine as well.

It is best to find an App that has most of the features already implemented. Only the remaining work need to be done.

#### Milestones

* Analyzing an existing or creating a new App
* add QR-Code scanner to add a contact
* establish an audio connection to an IP address
* your points..

##### PREPARATION/BONDING

- Good knowledge in Java (or whatever target language)
- Medium knowledge in Networking
