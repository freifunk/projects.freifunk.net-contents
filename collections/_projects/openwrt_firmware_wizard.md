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
name: "OpenWrt Firmware Wizard"
requirements:
  - "Web design"
  - "Programming"
  - "OpenWrt"
tags:
  - GSoC2019
  - OpenWrt
---

## Initial Firmware Retrieval

[OpenWrt](openwrt.org) is a Linux distribution for off the shelf WiFi routers. People who want to update their device, often do not know what firmware file to download. So far the best option is the Wiki, but it is often loaded with too much information. The file download organizes all images files by architecture, but that is what most user usually do not know beforehand. A website that helps to select the correct image and how to apply them will help the adoption of OpenWrt by less tech savvy people.

Required Features:

* Display device manufacturer / model name / hardware version / OpenWrt release / link to correct images
* Display a help for how to apply the image depending on its type (factory/sysupgrade image, rootfs/kernel image)
* Select model/images by typing in part of the device model name
* create images with different flavours (take functionality from Chef)

The plan here is to rewrite [Chef](https://github.com/libremesh/chef) from scratch and allow it to use stock OpenWrt images with a static selection of packages (from the OpenWrt download [sever](https://downloads.openwrt.org/) and also talk with the ASU server backend to create images with a specific feature set as Chef does already.

## Firmware Upgrades

Create a router web interface package for [LuCI](https://openwrt.org/docs/guide-user/luci/start) to check and apply new images. The [luci-app-attendedsysupgrade](https://github.com/openwrt/luci/tree/master/applications/luci-app-attendedsysupgrade) can be used as a template.

Required Features:

* Search for updates (downloads and checks json file)
* Apply update (apply `sysupgrade /tmp/image_sysupgrade.bin`)

## Create data

To get the data for both projects, the OpenWrt build system needs to modified to create json files with the necessary meta data.
There is an [example](https://git.openwrt.org/?p=openwrt/staging/lynxis.git;a=commitdiff;h=e2dd9c40cfea093aeb337fe66fe338f17543f118;hp=11590e7452bd61923c1339231df61fa0c539e025) avaialble on how to let the build system create json files.

#### Milestones

* Work out a plan with the specifics of tasks.
* Let the OpenWrt build system create JSON files. (GnuMake)
* Create a small tool to collect all JSON files in one JSON file. (Python or Shell script)
* Create a firmware wizard that could be integrated on openwrt.org to guide users. (HTML/JS)
* Create a LuCI package to search for updates and apply them. (Lua)

##### PREPARATION/BONDING

* Web development (html/js/css)
* Basic Lua knowlege
* Basic Knowledge of OpenWrt (should have compiled an image once before)
* Basic Makefile knowledge
