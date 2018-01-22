---
name: "nodewatcher: Node data matrix comparison module for nodewatcher"
desc: "The idea is to create a module which provides a page/matrix for node data comparison."
requirements:
 - "Python/Django, HTML/JavaScript experience."
difficulty: "medium"
mentors:
 - mitar
initiatives:
 - GSoC
tags:
 - nodewatcher
collaborating_projects:
 - wlanslovenija
---

The idea is to create a module which provides a page/matrix for node data comparison. Currently data is displayed only as a simple list of nodes with a fixed set of columns. The idea is to improve this so that custom columns can be added/removed. And also to add another dimension to get a matrix so that it is easy to compare values between nodes. For example, see how stability of nodes relate to number of clients. Additionally, this idea could be extended by an option to draw/plot selected columns/values as scatterplots.

You can see many data we collect as potential interesting and it would be interesting to be able to compare them. With matrix display this could be possible. So, a better way to compare nodes among themselves is wanted, and if possible to also visualize that.

Student should have experience or be willing to learn Python and Django and how to write Django apps together with basic understanding of HTML/JavaScript and general web development. 

#### Milestones

* Learn about the nodewatcher and nodewatcher API.
* Implement a reusable JavaScript code for display of data matrix.
* Integrate it with API and various places in nodewatcher as an option to view data in.
* Document and implements tests.
