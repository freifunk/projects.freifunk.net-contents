---
name: "OpenWrt Google Coral board support"
desc: "Integration of Google Coral board in Openwrt"
collaborating_projects:
  - openwrt.org
developers_involved:
  - schuza
difficulty: tough
status: open
initiatives:
  - GSoC
  - GSoC2023
issues:
size: "350 hours"
markdown: google_coral_board_support.md
mentors:
  - schuza
requirements:
  - "Ansi C"
  - "Ansi C++"
  - "ash"
  - "Python"
tags:
  - GSoC2023
  - OpenWrt
  - machine learning
  - CNN
  - Linux Kernel
---

The Coral Board integrates a Google Coral Edge Tensor Processing Unit (TPU) as Mini PCIe Accelerator [1], 
M.2 Accelerator A+E key or via USB. The TPU can be leveraged to run TensorFlow Light models on embedded systems. The goal is to integrate the board and environment into the OpenWrt build environment [2].

Moreover, within the GSoC project, the task is to come up with a simple example [3] to demonstrate the capabilities of the Coral board. Thus, the goal is to develop and evaluate some use cases such as device fingerprinting etc.

Accordingly, the participant will first integrate the board into the OpenWrt environment, design and describe possible use cases, and realize a use case that shows the benefits of the TPU.

#### Resources

* [1] https://coral.ai/products/pcie-accelerator
* [2] https://openwrt.org/
* [3] http://trac.gateworks.com/wiki/TPU
* [4] https://coral.ai/docs/edgetpu/models-intro


#### Milestones

* Integration plan for the Coral board in the OpenWrt build environment
* Integration of the tools and drivers into OpenWrt
* Description of different use cases that leverage the capabilities of the Google Coral Edge Tensor Processing Unit (TPU)
* Implementation of a dedicated use case that demonstrates the benefits of the TPU

##### PREPARATION/BONDING

* Understanding of the OpenWrt build environment
* Understanding of convolutional neural networks (CNN) and frameworks

##### Coding Period

* Integration of the Coral board support into OpenWrt
* Implementation of a use case
* Evaluation of the use case
* Demonstration of the benefits
