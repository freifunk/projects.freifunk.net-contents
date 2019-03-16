---
collaborating_projects:
  - openwrt
desc: "Create a wizard to select the correct firmware for your router for openwrt.org"
developers_involved: [ ]
difficulty: low
status: open
initiatives:
  - GSoC
issues:
markdown: openwrt_firmware_wizard.md
mentors:
  - mwarning
  - aparcar
name: "OpenWrt Firmware Wizard"
requirements:
  - "Web design"
  - "Programming"
  - "OpenWrt"
tags:
  - GSoC2019
  - OpenWrt
---

[OpenWrt](openwrt.org) is a Linux distribution for off the shelf WiFi routers. People who want to update their device, often do not know what firmware file to download. So far the best option is the Wiki, but it is often loaded with too much information. The file download organizes all images files by architecture, but that is what most user usually do not know beforehand. A website that helps to select the correct image and how to apply them will help the adoption of OpenWrt by less tech savvy people.

There are a few projects already with slightly different aims/problems:

- [Chef](https://github.com/libremesh/chef)
  - builds images rather then offering images
- [Gluon Firmware Selector](https://github.com/freifunk-darmstadt/gluon-firmware-selector)
  - targets Gluon OpenWrt flavored images only (with a slightly different image names and only a few image names)
- [Firmware Selector](https://github.com/freifunk-bielefeld/firmware-selector/)
 - similar to the gluon version
 - maps the entire OpenWrt image list with the help of a currated list of matchers that needs to be curated.

The current problem is that no project is suitable for openwrt.org right now. The main problem is the source of the information. A external database quickly gets old. The information from the wiki is hard to extract, incomplete and inflated. Therefore, the most reasonable solution seems to be to add meta data to the OpenWrt database. The idea is to create a JSON file as part of the OpenWrt build.

The project falls into two parts:

1. Create web interface:
  - Data comes from a JSON file
  - Display device manufacturer / model name / hardware version / OpenWrt release / link to correct images
  - Display a help for how to apply the image depending on its type (factory/sysupgrade image, rootfs/kernel image)
  - Select model/images by typing in part of the device model name
2. Extend OpenWrt build system:
  - Add metadata
  - Output JSON file

These tasks requires communication with the OpenWrt community for everything that adds changes to OpenWrt/openwrt.org.
Task 1. will probaby be 1/3 of the work, task 2. will consume about 2/3 of the project time.

A good preparation would be to try to build OpenWrt. The [OpenWrt Wiki](https://openwrt.org/docs/start) is a good start.

#### Milestones

* Understand the current web interfaces to salvage them if useful
* Understand the basics the OpenWrt build system
* Speak with the OpenWrt community to decide on the metadata that OpenWrt should output
* Create a web interface that could be integrated on openwrt.org to guide users

##### PREPARATION/BONDING

- Communication with the OpenWrt community
- Basic knowledge of web development (html/js/css)
- Medium knowledge of the OpenWrt system (compile and use OpenWrt)
- Basic Makefile knowledge
