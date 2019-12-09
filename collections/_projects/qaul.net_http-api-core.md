---
name: "qaul.net HTTP API Core Application Logic"
desc: "Develop qaul.net HTTP API and core application logic."
collaborating_projects:
  - qaul.net
developers_involved: []
difficulty: medium
status: completed 
initiatives:
  - GSoC
issues: https://github.com/qaul/qaul.net/issues/236
markdown: qaul.net_http-api-core.md
mentors:
  - spacekookie
  - mathjud
  - luxferresum
requirements:
  - "Rust programming language"
  - "Rough knowledge of json:api"
  - "Software Architecture"
tags:
  - GSoC2019
  - qaul.net
  - Rust
  - HTTP API
---

`qaul.net` is a mesh networking communication app that has been around since 2011
with active users around the world, using it instead of traditional internet
infrastructure to share files, data and communicate.

The project is now undergoing a complete re-write in Rust in order to support
more modern hardware, be more maintainable and extendable.
We are searching for students who want to be a part of this rewrite in the
early stage, with the idea to become longer term contributers to the project.

One area of work is around the new HTTP API which will allow interfacing with
a web front-end.
Someone working on this project would be responsible for not only implementing
the API with `json:api` in Rust, but also some of the the underlying core components
of the `qaul.net` library for user and message management, working closely together
with the rest of the team.



#### Milestones

* Implement HTTP API in Rust
  * Decide on the details of the HTTP API
  * Ensure compatibility with the new Web GUI
* Design & Implement message management
* Implement configuration management


##### PREPARATION/BONDING

* Get a general understanding of how qaul.net works
* Get a general understanding of the `libqaul` core APIs
* Learn about `json:api`
* Pick out an HTTP library to use for the implementaiton
* Discuss possible development with mentors
