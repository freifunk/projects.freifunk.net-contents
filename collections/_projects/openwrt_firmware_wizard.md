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

The current problem is that no project is suitable for OpenWrt right now. The project should aim for minimal/no manual updates in case of a new OpenWrt release.

Tasks:
 - Collect image information
   - ideal would be to create the desired JSON files as part of the openwrt build system (proposals are available)
   - Fallback approach: Scrape information from OpenWrt sources and/or the website/wiki
 - create a website:
   - Display device manufacturer / model name / hardware version / OpenWrt release / link to correct images
   - Display a help for how to apply the image depending on its type (factory/sysupgrade image, rootfs/kernel image)
   - Select model/images by typing in part of the device model name

These tasks require communication with the OpenWrt community for everything that adds changes to OpenWrt/openwrt.org.

#### Milestones

* Identifiy the different approaches to get the image file information
* Make that information available in a desired format (e.g. JSON)
* Create a website that could be integrated on openwrt.org to guide users

##### PREPARATION/BONDING

- Web development (html/js/css)
- Basic Knowledge of OpenWrt (should have compiled an image once before)
- Basic Makefile knowledge
