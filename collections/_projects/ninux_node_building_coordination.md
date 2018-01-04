---
collaborating_projects:
  - ninux
desc: "Implement a Web platform to coordinate wireless community network nodes deployment"
developers_involved: []
difficulty: medium
status: open
initiatives:
  - GSoC
markdown: ninux_node_building_coordination.md
mentors:
  - clauz
name: "Node building coordination Web platform"
requirements:
  - "Web programming"
  - "Software Design"
  - "Python, django"
tags:
  - web
  - communities
  - nodes
  - django
---

Building a community network node is often a task that cannot be accomplished by a person alone. The typical process of node building in the ninux.org community network goes through the following phases:

* the future node owner performs a survey of the location (i.e. the roof of her house/building) and takes pictures
* the feasibility of the node building and the establishment of links to other nodes is assessed by other members of the community network
* if it's feasible, the node owner buys the devices to be installed (or takes them from the community network common pool)
* the node installation is planned in advance: the tools to use, the hardware (poles, ties, etc.) to employ, the number of people needed to perform the installation (help from other community network members is essential for node installation)
* a date and time is decided for the installation 

Today community network members use a set general purpose online tools (e.g. mailing list, doodle, chat) to schedule and organize node installations. This can be sometimes frustrating as it might be difficult to get an overview and track the user activities.

We believe that the development a Web platform targeted to the specific purpose of coordinating and planning node building could benefit all community networks over the World. The platform should:

* allow the future node owner to create a description of the node installation environment (location on the map, survey pictures, links) and a target number of volunteers to help
* allow to choose a common date, time and place between the node installation participants for the node installation
* allow interaction (e.g. comments) between node installation participants
* allow a global view of the number of missing volunteers to reach the set target for each node installation, so that others willing to contribute can jump in
* allow the export a calendar (e.g. in ics format) with the scheduled installations


#### Milestones

##### PREPARATION/BONDING

- Understand how community network node deployment works in terms of "workflow" and the currently employed tools, by e.g. joining the ninux chat

