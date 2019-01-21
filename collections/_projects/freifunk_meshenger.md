---
collaborating_projects:
  - freifunk
desc: "Extend the Local Phone App to allow phone calls over the Internet"
developers_involved: [ ]
difficulty: medium
status: open
initiatives:
  - GSoC
issues:
  - layout problems with smaller screens
markdown: meshenger.md
mentors:
  - mwarning 
name: "Local Phone App"
requirements:
  - "Analyzing and coding"
  - "Programming"
  - "Networking"
tags:
  - app
  - GSoC2019
  - android
  - webrtc
---

This is a follow up project of last years [Local Phone App](https://projects.freifunk.net/#/projects?project=local_phone_app&lang=en). The current state of the App is available on (F-Droid)[https://f-droid.org/packages/d.d.meshenger/]. The projects aim was to provide a usable Android App that allows local video/audio communication on local networks without any intermediate servers or presence of the Internet.

While the project was a success, some useful features and polishing is missing. Here is a list of desired feature suggestions:

- The possibility to call contacts over the Internet as a fallback. Otherwise the App will be too specialized for people to be used at all. WebRTC allows the possibility to use public or own servers to facilitate direct connections over the Internet. But that feature is currently not used / disabled for all calls. This might be relatively easy to achieve as WebRTC already has most of the features.
- Communication by chat option. This could also be made to work by forwarding messages (also called delay tolerant networking). A useful technology here might be [Secure Scuttelbut](https://github.com/ssbc). 
- Secure Authentication. Currently, there is no authentication to initial handshake. The Phone/Video data is already encrypted.
- Use a standardized WebRTC signaling. [Matrix](https://matrix.org/blog/home/) might offer a possible idea here. 
- App polishing/bugfixing. For example, fix app for new Anroid versions and fix situations when a call gets interrupted because the screen turns off.
- Show own Camera feed in a small window during video calls.

#### Milestones

* Allow contacs with target hostname (e.g. mydomain.com) and WebRTC signaling servers.
* Allow calls over the Internet with optional STUN/TURN servers.
* Allow an easy setup of own signaling servers.
  * This is probably more of a find and document task, as there are existing open source solutions.
* Allow text messaging.
* Polishing of the current code.
* Adaptation to known android development patterns (different bitmaps for different resolutions, ...).

##### PREPARATION/BONDING

- Good knowledge in Android development.
- Knowledge of WebRTC basics.
- Overview of current (decentralized/federated) available communication technologies.
- Medium knowledge in Networking
