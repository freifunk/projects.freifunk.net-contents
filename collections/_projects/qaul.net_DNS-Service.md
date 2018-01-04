---
collaborating_projects:
  - qaul.net
desc: "Create a qaul.net wide DNS service to address network services via DNS"
developers_involved: []
difficulty: high
status: open
initiatives:
  - GSoC
issues:
  - "https://github.com/qaul/qaul.net/issues/210"
markdown: qaul.net_DNS-Service.md
mentors:
  - MathJud
name: "Implement .qaul DNS Service"
requirements:
  - "Analyzing and coding"
  - "C"
  - "DNS Protocol"
  - "http protocol"
tags:
  - C
  - DNS
  - Networking
---

qaul.net has an existing DNS stub which handles the captive portal. 

The task is to create a qaul.net wide decentralized, user centric DNS system which resolves user names via 'username.qaul' host name scheme. This is helpful to easily address user services within qaul.net.

This requires several steps:
* DNS daemon
* Decentralized DNS maintenance (via qaul service protocol)
* Virtual hosts in web server
* User configurable port forwarding


#### Milestones

* Create a DNS API
* Implement the user deamon
* Update DNS deamon via qaul.net
* Create user centric virtual hosts
* Make virtual hosts configurable
* Implement virtual host based port forwarding


##### PREPARATION/BONDING

* Understand the DNS protocol
    * DNS puny code
* Analyze all the interaction points of DNS services in qaul.net
    * Analyze DNS host system integration
    * Analyze Web Services
