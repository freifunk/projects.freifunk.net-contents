---
name: Ad-Hoc Mesh Networks with Satellites
desc: Create a virtual satellite scenario to test various mesh routing protocols. 
maskdown: freifunk-for-satellites.md
collaborating_projects:
  - freifunk
developers_involved: []
difficulty: medium
size: "175 hours"
status: open
email: moritzwarning@web.de
initiatives:
  - GSoC2022
issues:
mentors:
  - mwarning
requirements:
  - "Python and Shell programming"
  - "Networking basics"
  - "A bit of simplified orbital mechanics"
tags:
  - GSoC
  - Linux
  - Satellites
  - Mesh Networking
---

[Starlink](https://www.starlink.com/) has shown that Internet access via Satellites becomes a reallity now. While it would be interesting to run mesh networks on Satellites, they are still a bit pricy. Thus we will create a simulation and see how commonly used routing protocols would run on a Satellite network.

The task will be to create 1-3 tests for [Meshnet-lab](https://github.com/mwarning/meshnet-lab). There are already a few working tests there to build up on. This GSoC project will consist of three parts:

1. design test scenarios
2. implement tests with Python (example [Convergence test](https://github.com/mwarning/meshnet-lab/blob/master/tests/convergence1/run.py)
3. run tests to create result graphs with Python [matplotlib](https://matplotlib.org/stable/gallery/)

Possible test scenarios:
- random satellites around a round Earth
- Starlink like satellite constellations
  - maybe even use real satellite data :-)
- Deep Space Network

Let's see how mesh routing protocols like those used for [Freifunk](https://freifunk.net) and others, of course, would work in space. The amount of realism for this project is limited, but it is valuable for the future development

The student should be comfortable with Python, basic Linux networking commands (e.g. `ip`) and a bit of Matrix multiplication (rotation Matrices). 

Many other aspects of this project are up for the discussion. If you are just interested in the topic or are unsure if this is something for you, then feel free to contact the mentor(s) beforehand. moritzwarning@web.de :-)

#### Milestones

##### GSoC Peparation/Bonding

* Run first very basic tests with existing software and get to know the outline of the software stack.
* Get comfortable with existing mesh routing software. This requires running the mesh software and see how they tick.
* Talking about the outline of the project.
* Maybe visit the Battlemesh (depends on Covid restrictions, date&location).

##### GSOC Start

* Design test scenarios (what and how to test)
* Start implementation in Python. 
* Plan more fine grained milestones.

##### GSOC Midterm

* Implement tests scenarios.
* Start running the tests.

##### GSOC Final

* Run test scenarios and fix any upcoming problems.
* Generation of results in the form of graphs/animations.
