---
collaborating_projects:
  - freifunk
  - openwifi
  - openWLANmap
desc: "Develop a new OpenWLANMap wardriver App wich is compatible to newer Androids"
developers_involved: [ Jan-Tarek Butt, Казанцев Егор ]
difficulty: medium
status: open
initiatives:
  - GSoC
issues:
  - "https://github.com/openwifi-su"
  - "https://sourceforge.net/p/libwlocate/code/ci/master/tree/master/android/"
markdown: freifunk_openwifi_wardiver_app.md
mentors:
  - Jan-Tarek Butt
  - (Казанцев Егор)
name: "Develop a new OpenWLANMap wardriver App wich is compatible to newer Androids"
requirements:
  - "Analyzing, design and coding"
  - "Java"
  - "Math"
tags:
  - geolocation
  - json
  - api
  - map
  - collectors
  - communities
---

The wardriver application is one of the fundamental base structures of the WLAN mapping function from openwifi.su
This application collects surrounding WiFi information of phones and bind GPS coordinates on this data. This data will
send to our backend which integrate this into a database. Devices like freifunk routers can receive its position base on
given surrounding  WiFis and requesting this data to the server backend. This WiFi was done by the last Google Summer of Code 2017
in the project https://blog.freifunk.net/2017/08/29/geolocator-software-defined-gps-final-evaluation/
The actual OpenWLANMap App is hardly out of date and have an extremely bad performance.

The target is to build a new war driver App wich is also compatible to newer Androids. Furthermore this application and the API behind that is not or not well documented. This should also be done during the GSoC18. This will give the location project a better base.

Necessary keywords are:

* Analyzing old API design
* create new API (if necessary)
* hold backwards compatibility
* force collecting minimized data.
* force collecting only necessary data related for location
* always keep an eye on privacy e.g. "_onmap"
* save phone resources e.g. akku, wakups..
* your points..

#### Milestones

##### PREPARATION/BONDING

- Good knowledge in Java
