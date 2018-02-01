---
collaborating_projects:
  - freifunk
name: "VRConfig"
desc: "Create a Visual Router Configuration for OpenWrt"
developers_involved: []
difficulty: hard
status: open
initiatives:
  - GSoC
issues:
markdown: freifunk_visual_router_config.md
mentors:
  - thuehn
requirements:
  - "Analyzing, design and coding"
  - "Luci"
  - "Lua"
  - "OpenWrt build system & per target package make management"
  - "Java or Javascript"
tags:
  - Luci 
  - web interface
  - openwrt
  - usability
---

The current Luci Webinterface puts a certain and quite high knowledge barrier to the endusers in terms of simplicity of configuration.
This project aims to improve the usuablity of the Luci Webinterface by introducing a new visual configuration system tailored to each individual router.
The main goal of VRConfig is a new abstraction between a real picture of the current router model with its actual ports, buttons, LED layout and their representation within Luci.
VRConfig will allow the community to collect images of each router platform and to annotate the location of Ethernet ports, WiFi antannas, USB ports, LEDS, serial line, buttons, switch, power plugs, ect.
Based on such an annotated router image, a new visual configuration application in LUCI will be developed. 
In the end the user will be able to interact with his router via its visual representation in the Luci webinterface., e.g. clicking on a port to configure it, visual feedback if ethernet cable is conected, ect.


#### Milestones

- Investigate suitable image and metadata file formats (size implication, flexibilty)
- Intergration of the image & metadata files into the current openwrt buildsystem and packagemanagement system
- Community application to colect and annotate different router platforms
- Luci demo application based on the new visuals

##### PREPARATION/BONDING

- Investigate most suitable technology for image annotation application
- Get an overview of which images of a router are needed for the visual configuration interface
