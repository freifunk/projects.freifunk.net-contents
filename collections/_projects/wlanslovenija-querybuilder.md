---
name: "nodewatcher: nodewatcher API and datastream query builder"
desc: "Implement a dynamic query builder for nodewatcher API."
requirements:
 - "Python/Django, HTML/JavaScript experience."
difficulty: "medium"
mentors:
 - mitar
initiatives:
 - GSoC
tags:
 - GSoC2018
 - nodewatcher
collaborating_projects:
 - wlanslovenija
---

nodewatcher collects a lot of data from nodes and exposes it through an API called [datastream](https://github.com/wlanslovenija/django-datastream). Moreover it provides API to access its [registry](https://nodewatcher.readthedocs.io/en/latest/registry.html) of nodes. Both APIs are powerful, but building queries against them requires a lot of knowledge.

Currently various ndoewatcher modules consume this data and make hard-coded queries to display it. The issue is that there is much more data available then currently displayed, but also not everything is interesting to everybody. Moreover, manually building URLs for queries against is complicated. So, the idea is to create a web interface for the query builder where users could create their own query by combining available fields, filters, sorting, and ways to display data. If they are satisfied, they could also store the query for others to use it.

Inspiration can be taken from [Trac query builder](https://dev.wlan-si.net/query) and how it allows to store made queries as [reports](https://dev.wlan-si.net/report).

This will probably be mostly a JavaScript client-side implementation, but reading and understanding the server-side API is also needed. 

#### Milestones

* Learn about the nodewatcher and its API.
* Learn more about JSON-LD and how it can help to desribe JSON documents and APIs.
* Implement a simple verison of the query builder on top of nodewatcher API.
* Extend the simple verison with support for datastream plots as one of output types.
* Integrate it with nodewatcher as a nodewatcher module.
* Document and implements tests.
