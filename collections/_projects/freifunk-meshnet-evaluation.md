---
name: Freifunk Meshnet Protocol Evaluation
desc: Develop a virtual testbed and test various mesh routing protocols
maskdown: freifunk-meshnet-evaluation.md
collaborating_projects:
  - battlmesh
  - freifunk
developers_involved: []
difficulty: medium
status: open
email: moritzwarning@web.de
initiatives:
  - GSoC
issues:
mentors:
  - mwarning
requirements:
  - "Python and Shell programming"
  - "Advanced networking knowledge"
  - "Mesh networking software basics"
tags:
  - GSoC
  - Linux
  - Networking
  - batman-adv
  - BABEL
  - OLSR
  - Yggdrasil
---

For a network community to consider new mesh routing protocols, it is necessary to do extensive testing.
But real life tests results are hard to make comparable. Mobility scenarios are hard to replicate and to test properties such as network scalabilty is almost impossible due to the costs of hardware nodes.

To help users and developers of mesh networking software, a tool should be developed to alleviate this problem. By a "press of a button", a series of tests should be run on a computer and result in different graphs that contain data from different mesh network protocols. As part of this project, test setups needs to be defined in terms of topology, link quality and changes in time (in JSON). These defined test setups need to be implemented using Linux Network Namespaces and run for protocols such as [B.A.T.M.A.N.-adv](https://www.open-mesh.org/projects/batman-adv/wiki), [Babel](https://www.irif.fr/~jch/software/babel/), [OLSR](https://www.olsr.org) and [Yggdrasil](https://yggdrasil-network.github.io/). Other protocols can be added as the student sees fit. The scenarios to be tested should cover reachability, scalability, throughput and mobility resistance. But can be limited if time becomes limited.

A project to create a virtual mesh network on your local computer running Linux is [already available](https://github.com/mwarning/meshnet-lab) if the student choses to make use of this particular one. While it can run all the mentioned mesh routing protocols, many parts are missing, such as a generator for different complex topologies (or any import of existing topologies from Freifunk). Any handling of mobility is also missing.

The main goal of the project would be to have reproducible results from different routing protocols that can be presented to the [Freifunk](https://freifunk.net)/[Battlemesh](https://battlemesh.org/) community in the form of nice graphs.

A secondary goal is to make the test run as simple as possible to give a useful tool to everyone interested.

The student should be comfortable with existing Linux networking commands like ip or tc and should know how e.g. what a switch is different from a hub and how networks work. Existing mesh networking experience is welcome. Most programming aspects will be done in Python.

Many aspects of this project are up for the discussion. Contacting the mentor(s) beforehand is welcome and shows iniative (moritzwarning@web.de). :-)

#### Milestones

##### GSoC Peraration/Bonding

* Run first very basic tests with existing software and get to know the outline of the software stack.
* Get comfortable with existing mesh routing software. This requires to ask around within the community.
* Talking about the outline of the project.
* Maybe visit the Battlemesh (depends on date/location).

##### GSOC Start

* Define the format of test scenarios.
* Plan more fine grained milestones.

##### GSOC Midterm

* Implement network setup tools.
* Make different mesh routing protocols run.
* Aquire/Generate different test scenarios.

##### GSOC Final

* Run test scenarios and fix any upcoming problems.
* Generation of results in the form of graphs.
