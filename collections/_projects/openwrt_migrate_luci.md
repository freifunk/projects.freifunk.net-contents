---
name: "LuCI migrate to js-based framework"
desc: "Migrate LuCI apps, modules and pages to the new javascript API"
collaborating_projects:
  - openwrt.org
developers_involved:
  - jow
  - aparcar
difficulty: medium
status: completed 
initiatives:
  - GSoC
  - GSoC2023
issues:
  - https://github.com/openwrt/luci/issues/3378
size: "175 hours"
markdown: openwrt_migrate_luci_javascript.md
mentors:
  - andibraeu
requirements:
  - "html"
  - "lua"
  - "javascript"
  - "ash"
tags:
  - GSoC2023
  - OpenWrt
  - UI
  - configuration
---

`OpenWrt` is a distribution for embedded devices such as WiFi router etc. `LuCI` is a framework to build a web interface for configuration and monitoing.

With the old system all pages are rendered on the router delivering html to the browser. This leads to a higher load on the embedded devices. To reduce this load, rendering should be outsoruced to the browser. The framework LuCI itself is already prepared for this and provides a client side API.

Data will be provided via rpcd and ubus in a JSON format. You probably have to write new rpcd services to provide data that was formerly used directly on the router. Services are usually written as ash script.

#### Resources

* LuCI [source code](https://github.com/openwrt/luci)
* LuCI [documentation](https://github.com/openwrt/luci/wiki/Documentation)
* client-side JavaScript API [documentation](https://openwrt.github.io/luci/jsapi/)
* Freifunk [apps and modules](https://github.com/freifunk/openwrt-packages) for LuCI
* [Another app](https://github.com/weimarnetz/packages/tree/brauhaus-19.07/utils/luci-app-weimarnetz) already migrated to js

#### Milestones

* Learn how the new LuCI client side API works
* Learn how to write rpcd services
* Learn how to set permissions and menu entries
* Discuss a list of LuCI apps and modules you plan to migrate
* Make a HowTo for others to help them migrating further apps


##### PREPARATION/BONDING

* Get a general understanding of how the cbi based (old) approach works.
* Study the [example app](https://github.com/openwrt/luci/tree/master/applications/luci-app-example) to see how it generally works.
* See other apps like [luci-mod-freifunk](https://github.com/freifunk/openwrt-packages/tree/master/modules/luci-mod-freifunk) that are already migrated to learn more details.
* Get familiar with rpcd and ubus.

##### Coding Period

* Find a simple app to start migrating
* Create documentation for things that have not been documented so far
* Work step by step on the list of apps and modules you created in the beginning
