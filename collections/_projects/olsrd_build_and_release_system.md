---
name: "Build, test and release OLSRd v1"
desc: "Add tests and create a build and release system"
collaborating_projects:
  - olsrd
developers_involved:
  - PolynomialDivision
difficulty: medium
status: open
initiatives:
  - GSoC
  - GSoC2023
issues: []
size: "175 hours"
markdown: olsrd_build_and_release_system.md
mentors:
  - PolynomialDivision
  - andibraeu
requirements:
  - "C"
  - "Makefile"
  - "github actions"
  - "bash"
tags:
  - GSoC2023
  - OLSRd
  - Legacy
  - build
  - release
  - testing
---

The Optimized Link State Routing Protocol (`OLSR`) is an IP routing protocol optimized for mobile ad hoc networks, which can also be used on other wireless ad hoc networks. 

`OLSR` was one of the first protocols created nearly 20 years ago. For some use cases, it's still a reliable and stable protocol and is still used in several wireless network communities.

However, further development and bug fixing is getting more and more complicated due to a legacy codebase. One step in the right direction would be to add automated building and testing as well as an easier release system.

#### Resources

* OLSR [information](https://en.wikipedia.org/wiki/Optimized_Link_State_Routing_Protocol)
* OLSR [Website](http://www.olsr.org/mediawiki/index.php/Main_Page)
* [Source Code](https://github.com/OLSR/olsrd)

#### Milestones

* Find a test framework to enable automated testing for release candidates and add first tests
* Extend testing to modules and libs
* Develop workflows to run tests and build a release


##### PREPARATION/BONDING

* Understand the current release process and identify steps.
* Find the modules that need to be released.
* Evaluate how to test releases. Probably unit tests are too complex, but you could add integration or end-to-end tests.
* Understand how we can use Github Actions or other tools can be used for continuous integration.
* Find tools that help monitor the code quality.

##### Coding Period

* Discuss with your mentors what parts need to be released
* Develop a method to test the software. We'll use the results in a decision if we draft a new release.
* Adopt Makefiles and add scripts to enable continuous integration.
