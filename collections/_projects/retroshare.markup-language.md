---
name: "RetroShare implement simple Markup Language support"
desc: "Move away from sending HTML over the network, to avoid security risc and improve performances and interoperability"
markdown: retroshare.markup-language.md
collaborating_projects:
  - retroshare
developers_involved:
  - PhenomRetroShare
  - sehraf
difficulty: medium
status: open
initiatives:
  - GSoC
issues:
  - https://github.com/RetroShare/RetroShare/pull/999
  - https://github.com/RetroShare/RetroShare/pull/1304
mentors:
  - csoler
  - G10h4ck
requirements:
  - "Analyzing and coding"
  - "C++"
  - "Qt"
tags:
  - GSoC
  - C++
  - Qt
  - AsciiDoc
  - Markdown
---

Most of user-input texts in the Retroshare software are supplied to the backend
as HTML by Qt. Although it offers a lot of possibilities, it is also a double
weakness both in terms of security and CPU-efficiency. The plan is therefore to
implement a markup language (ex. a subset of AsciiDoc or Markdown) translation
which would ensure that a only minimal set of features can be represented and
displayed (emoticons, links, images, font-style bold, italic...).

RetroShare-gui should accept markup text to be displayed and convert it
internally into proper HTML that Qt will understand.
Possibly ensure some minimal backward compatibility with the existing data.

#### Milestones

* define the list of features we want to be handled by the markup language
* define a new text editing widget/component that has the needed buttons and options to handle markup text (e.g. link and image insertion).
* implement an approximate conversion of existing html into this language for backward compatibility

##### PREPARATION/BONDING

* get familiar with the RetroShare network
* understand how text is supplied by users and converted into HTML
* discuss possible options with the developers

