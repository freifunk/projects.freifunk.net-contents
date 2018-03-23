---
collaborating_projects:
  - freifunk
  - openwifi
  - openWLANmap
desc: "Develop a new OpenWLANMap wardriver App which is compatible to newer Androids"
developers_involved:
  - "Jan-Tarek Butt"
  - "Казанцев Егор"
difficulty: medium
status: open
initiatives:
  - GSoC
issues:
  - "https://github.com/openwifi-su"
  - "https://sourceforge.net/p/libwlocate/code/ci/master/tree/master/android/"
markdown: freifunk_openwifi_wardiver_app.md
mentors:
  - 2tata
  - saintbyte
name: "Develop a new OpenWLANMap wardriver App which is compatible to newer Androids"
requirements:
  - "Analyzing, design and coding"
  - "Java"
  - "Math"
tags:
  - GSoC2018
  - geolocation
  - json
  - api
  - map
  - collectors
  - communities
  - android
  - app
---

The wardriver application is one of the fundamental base structures of the WLAN mapping function from openwifi.su
This application collects surrounding WiFi information of phones and binds GPS coordinates on this data. This data will be
sent to our backend which integrates this into a database. Devices like freifunk routers (WIFI only) can receive its position base on
given surrounding  WiFis and request its position by sending this WiFi data to the server backend. This request mechanism was done by the last Google Summer of Code 2017
in the project https://blog.freifunk.net/2017/08/29/geolocator-software-defined-gps-final-evaluation/
The actual OpenWLANMap App is hardly out of date and has an extremely bad performance.

The target is to build a new wardriver App which is also compatible to newer Androids. Furthermore this application and the API behind that is not or not well documented. This should also be done during the GSoC18. This will give the location project a better base.

Necessary keywords are:

* Analyzing old API design
* create new API (if necessary)
* hold backwards compatibility
* force collecting minimized and only necessary data related for locations e.g. RSSI
* precaluclate as much as possebile on phones to reduce mobile bandwidth wasting.
* always keep an eye on privacy e.g. "_nomap"
* save phone resources e.g. akku, wakups..
* your points..

#### Milestones

##### PREPARATION/BONDING

- Good knowledge in Java
