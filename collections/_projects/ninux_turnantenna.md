---
collaborating_projects:
  - ninux
desc: "Re-write the code for the Turnantenna project"
developers_involved: []
difficulty: medium
status: completed
initiatives:
  - GSoC
markdown: ninux_turnantenna.md
mentors:
  - leonardomaccari
name: "Re-write the Turnantenna code"
requirements:
  - "Python Programming"
  - "Driver programming"
  - "Python, possibly PHP"
tags:
  - GSoC2018
  - engine
  - antenna
  - Orange Pi
---
The goal of the turnAntenna project is to realize the software needed to drive the "Turnantenna", a device that is able to automatically point an antenna in a specific direction.

The turnantenna is made of a step-by-step engine which moves  a bracket on which the antenna is placed. Below the bracket there is a box containing an Orange Pi board that drives the engine. The OPi is powered over ethernet, and contains a python code that is used to move the engine, and re-point the antenna. 
The basic idea is that in some cases you want to re-point an antenna mounted in a position that is not easily accessible, or you may want to re-point an antenna temporarily to do a test, and move it back. In this cases the turnantenna is useful because it can move the anenna without the need of physical access (i.e. the antenna is mounted on a 6 meters pole and you don't want to bring it down and up again). 
A few pictured of our current prototype can be found in this [presentation](https://github.com/ninux-fi/projects.freifunk.net-contents/blob/master/collections/_projects/girantenna.pdf)

The current code of the Turnantenna is made of two parts, a Python code that controls the engine, and a php page that is the user interface. Both projects are currently on github: [driver](https://github.com/ninux-fi/punter_node_driver), [Web Interface](https://github.com/ninux-fi/punter_node_web). Both projects need a rewrite, the driver is a collection of code from various sources and it needs to be improved, refactored and tests need to be added. The website needs a better shape.


#### Milestones

* replicate the system in your place. 
* re-write the driver code, cleaning up the code, adding tests achieving full code coverage, and documenting the code in Python
* write a full documentation for the whole project, document the software and hardware components in detail, write an how-to to reproduce the Turnantenna 
* improve the web interface. Actually, this should be re-wrote from scratch, but this task may not fit the time of a GSoC.

##### PREPARATION/BONDING

* Understand how the turnantenna works, enter in contact with the designers (the ninux community of Florence), understand how the system works.
* Possibly buy some low price devices (an Opi and a step-by-step engine, for less than 50€).
* Define with the mentor the precise deadlines of the sub-task

