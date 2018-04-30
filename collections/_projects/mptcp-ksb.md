---
name: "MultipathTCP and OpenWRT: port the Kernel Socks Bouncer (KSB) from Linux kernel 2.6 to 4.X"
desc: "Port the Kernel Socks Bouncer (KSB) from Linux kernel 2.6 to 4.X"
requirements:
 - "networking experience, C"
difficulty: "medium"
status: in_progress
mentors:
 - zoobab
initiatives:
 - GSoC
tags:
 - GSoC2018
 - mptcp
 - ksb
 - socks
 - openwrt
---

[Kernel Socks Bouncer](http://ksb.sourceforge.net/) is a Linux Kernel 2.6.x Loadable Kernel Module that that redirects tcp connection (to user-defined target hosts) through socks 4/5 chains. ksb26 is subdivided into a lkm [Linux Loadable Kernel Module] and a userspace manager. ksb26 lkm intercepts and redirects tcp connections. ksb26manager keeps updated socks list and loads target hosts list via character device.

During last year [port of MultipathTCP to LEDE/OpenWRT](https://github.com/spyff/lede-mptcp), we found that the speed bottleneck was in the context switching (between user space and kernel space) of the SOCKS proxy, [shadowsocks-libev-nocrypto in our case](https://github.com/spyff/shadowsocks-libev-nocrypto). When we presented our project at the OpenWRT Summit in Prague, we heard about about a similar implementation using a custom socks proxy entirely in kernel space.

The aim of this GSoC project is to then port an existing kernel socks proxy to more recent kernel version, and tests the results on embedded hardware, reusing the MultipathTCP port to LEDE/OpenWRT that has been made last year. Student should have experience or be willing to learn C, compiling and running code for OpenWRT, have experience with networking stack (IPv4, NAT).

#### Milestones

* Learn about MultipathTCP
* Learn about KSB, make it run with a 2.6 kernel
* Implement KSB support for a recent LTS kernel (4.9) to start with
* Document and implements performance tests on embedded hardware
