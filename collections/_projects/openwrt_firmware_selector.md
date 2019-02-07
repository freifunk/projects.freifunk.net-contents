---
collaborating_projects:
  - openwrt
desc: "Create a easy way to select the correct firmware for your router on openwrt.org"
developers_involved: [ ]
difficulty: low
status: open
initiatives:
  - GSoC
issues:
markdown: meshenger.md
mentors:
  - mwarning 
name: "OpenWrt Firmware Selection"
requirements:
  - "Web design"
  - "Programming"
  - "OpenWrt"
tags:
  - GSoC2019
  - OpenWrt
---

[OpenWrt](openwrt.org) is a Linux distribution for off the shelf WiFi routers. People who want to update their device often do not know what file to download. So far the best option is the Wiki, but it is often loaded with too many information. The file download organizes all images files by architecture. User usually do not know that beforehand. A website that helps to select the correct image and how to apply them will help the adoption of OpenWrt by less tech savvy people.

There are a few projects already with slightly different aims/problems:

- [Chef](https://github.com/libremesh/chef)
  - builds images rather then offering images
- [Gluon Firmware Selector](https://github.com/tecff/gluon-firmware-selector)
  - targets Gluon OpenWrt flavored images only (with a slightly different image names)
- [Firmware Selector](https://github.com/freifunk-bielefeld/firmware-selector/)
 - similar to the gluon version
 - maps the entire OpenWrt image list with the help of a currated list of matchers that needs to be curated.

The current problem is that no project is suitable for OpenWrt right now. The project should aim for minimal/no manual updates in case of a new OpenWrt release.

Tasks:
 - scrape information from OpenWrt sources and/or the website/wiki
   - this should run regulary and identify new OpenWrt releases and images
 - Display device manufacturer / model name / hardware version / OpenWrt release / link to correct images
 - Display a help for how to apply the image depending on its type (factory/sysupgrade image, rootfs/kernel image)
 - Select model/images by typing in part of the device model name

#### Milestones

* Identifiy the different sources for information (ask around etc.)
* Parse information in a desired format (e.g. JSON)
* Create a website that could be integrated on openwrt.org to guide users

##### PREPARATION/BONDING

- Ask around for all neded bits of information
- Knowledge of OpenWrt (should have compiled an image once before) 
- Web development (html/js/css)
