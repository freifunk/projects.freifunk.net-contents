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

This is a follow up project of last years [Local Phone App](https://projects.freifunk.net/#/projects?project=local_phone_app&lang=en). The current state of the App is available on [F-Droid](https://f-droid.org/packages/d.d.meshenger/). The projects aim was to provide a usable Android App that allows local video/audio communication on local networks without any intermediate servers or presence of the Internet.

While the project was a success, some useful features and polishing is missing. Here is a list of task suggestions, the last ones are less important/optional:

- App polishing/bugfixing. For example, fix app for new Anroid versions and fix situations when a call gets interrupted because the screen turns off.
- The possibility to call contacts over the Internet as a fallback. Otherwise the App will be too specialized for people to be used at all. WebRTC allows the possibility to use public or own servers to facilitate direct connections over the Internet. But that feature is currently not used / disabled for all calls. This task might be relatively easy to achieve as WebRTC already has most of the features. If this is not sufficient, [Matrix](https://matrix.org/blog/home/) or [ActivityPub](https://activitypub.rocks/) might offer a possible idea here.
- Secure Authentication. Currently, there is no authentication to initial handshake. The Phone/Video data is already encrypted.
- Communication by chat.
- Show own Camera feed in a small window during video calls.

This is just a list of suggestions and possible approaches. The main aim is to make the app more usable for mainstream usage.
Feel free to contact the mentor for further questions or even share own ideas on how to achive the tasks.

#### Milestones

* Get to know the current state of the code.
* Allow contacs with target hostname (e.g. mydomain.com) and enable STUN/TURN for those contacts.
  * This will allow making calls of the Internet.
* Allow an easy setup of own signaling servers.
  * This is probably more of a find and document task, as there are existing open source solutions.
  * An adaption of to common signaling formats might be a good idea here.
* Polishing of the current code.
* Your selection :-)

##### PREPARATION/BONDING

- Good knowledge in Android development.
- Medium knowledge of WebRTC.
- Good knowledge in Networking
- Overview of current (decentralized/federated) communication technologies might be helpful.
