---
collaborating_projects:
  - openwrt.org
desc: "Extend the openwrt PPA, or Personal Package Archive"
developers_involved: [ ]
difficulty: medium
status: open
size: "175 hours"
initiatives:
  - GSoC
  - GSoC2023
issues:
markdown: openwrt_ppa.md
mentors:
  - zoobab
name: "OpenWrt PPA Part 2"
requirements:
  - "Kubernetes"
  - "Docker"
  - "Shell"
  - "Makefiles"
  - "OpenWrt"
tags:
  - GSoC2023
  - OpenWrt
  - Kubernetes
  - Docker
  - Shell
  - Makefiles
---

[OpenWrt](openwrt.org) is a Linux distribution for off the shelf WiFi routers. People who want to make and distribute their personal packages, often for development purposes. So far the best option is to build the whole firmware from zero, but very few people use the OpenWrt SDKs. The idea behind this project is to create a platform to build and host those personal package repositories, possibility integrated with GIT farms, so that the end users can add a repositiory URL to use those packages, modelled on what Ubuntu PPA (Personal Package Archive) has been provided for years.

There is no such platform at the moment, packages are made via Pull Requests on a central repository, but that does not meet the requirements of a typical developer, which are:

1. Autonomy: no external person is needed to use the platform
2. Build with many different targets like: brcm2708, ath79, x86, sunxi, etc...
3. Generate an URL for each repository
4. CI/CD with green/red button: rebuild with latest commits
5. Optional: Deploy to a physical target device, or an emulator (see https://gitlab.com/zoobab/arduino-cli-esp8266)

Tasks:
 - Try the existing approaches, like cascading docker images (such as https://github.com/zoobab/openwrtsdkbuild)
 - Adapt OpenBuildService (OBS) to support the SDK

These tasks require communication with the OpenWrt community, notably to find out issues regarding the build system or the SDK.

#### Milestones

* Document existing tools and strategies
* Add support to Opensuse OpenBuildService (OBS), which already supports hosting packages for other distros (see this Github Issue "Add support for OpenWRT builds" https://github.com/openSUSE/open-build-service/issues/10228 and this "Howto add another package format to OBS" https://github.com/openSUSE/obs-build/blob/master/HOWTO.add_another_format)

##### Preparation

- Basic Knowledge of OpenWrt (should have compiled an image once before)
- Basic Makefile knowledge
- Basic Docker knowledge
