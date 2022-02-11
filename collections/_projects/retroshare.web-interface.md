---
collaborating_projects:
  - retroshare
desc: "Finalise the Retoshare Web Interface"
developers_involved: []
difficulty: easy
status: open
initiatives:
  - GSoC
  - GSoC2022
issues:
markdown: retroshare.embedded-friend-server.md
mentors:
  - csoler
  - G10h4ck
name: "RetroShare Create an embedded Tor-only friend server"
requirements:
  - "Javascript"
  - "Web design skills"
tags:
  - GSoC2022
  - Javascript
  - Web
---

Thanks to an automatically generated JSON API, it is now possible to interact with a running Retroshare node using http requests.
During previous GSoC sessions this communication system was leveraged to create a basic Web interface that allows Retroshare to run on a headless server,
while offering simple controls such as friend management, file transfer.

All the machinery that allows the Web interface to talk to a retroshare node is now well established, and most of the
work in this project will consist into creating the missing webpages (along with the associated JS code) to allow a remote user to 
work with the existing Retroshare services.

A lot remains to be done so that this interface can compare to the existing Qt interface. For this reason we do not expect the
applicants to fully finish the job, but to properly provide good designs and functional code for some parts of it. The following 
parts in particular should be a priority:
* files
* forums
* configuration
* channels


#### Milestones

This project requires the following steps:
* properly understanding how Retroshare and the web interface talk together
* choosing which parts of the interface the applicant would like to work on and for each of them,
* discussing some UI goals that suit the software's plan
* implementing the parts in the form of multiple pull requests that will be merged in the project.

##### PREPARATION/BONDING

We will only recruit applicants who made proper pull requests to https://github.com/Retroshare/RSNewWebUI before the 
selection process begins. The developer team can (and probably should) be contacted in order to get some ideas of simple contributions
to make at this step.

