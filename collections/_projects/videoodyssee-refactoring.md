---
collaborating_projects:
  - freifunk
desc: "Rebuild a media upload system"
developers_involved:
  - andibraeu
  - christian-draeger
difficulty: medium
size: "175 hours"
status: open
email: ab+gsoc2022@andi95.de
initiatives:
  - GSoC
  - GSoC2022
issues:
  - "https://github.com/freifunk/videoodyssee.freifunk.net-ci/issues/6"
  - "https://github.com/freifunk/videoodyssee.freifunk.net-ci/issues/2"
markdown: videoodyssee-refactoring.md
mentors:
  - andibraeu
  - christian-draeger
name: "videoodyssee: system refactoring"
requirements:
  - "Analyzing code and systems"
  - "evaluate solutions"
  - "refactoring, migrations"
  - "web design"
  - "kotlin, clojure, java, html, javascript, css"
tags:
  - GSoC2022
  - json
  - web
  - voctoweb
  - video
---

## About our videoodyssee

In 2017 we started our video portal for freifunk at [media.freifunk.net](https://media.freifunk.net). To get videos online we have a more or less complicated upload workflow:

1. upload video file to a processing server
2. correct video file settings
3. convert video to target formats
4. upload to CDN and Youtube
5. publish at the media portal

## Provided services

The following systems are involved:

1. [Videoodyssee Uploader](https://github.com/christian-draeger/videoodyssee-uploader) - a web portal to upload video files built with Spring Boot, Thymeleaf, CSS, JS, Ansible, and Maven
2. Videoodyssee - the processing server, built with bash scripts and python
3. [lambdacd pipeline](https://github.com/freifunk/videoodyssee.freifunk.net-ci/) - controls the workflow, built with Clojure, Leiningen, and LambdaCD
4. [mirrorbits](https://github.com/etix/mirrorbits) - the CDN, built with Go
5. [voctoweb](https://github.com/freifunk/voctoweb) - the media portal, built with Ruby, HTML, CSS, JS and puma

As of now, it is possible to upload new videos, but the process is not comfortable. So we need to improve the software.

## Ideas for changes

There are already some ideas for improvements:

* add publishing workflow to prevent the publishing of unwanted videos (e.g. send an email to a group of people to unlock the video)
* refactoring the uploader project to use a message-based frontend to a backend system, e.g. by using Spring Webflux, React or Websockets
* support multiple workers for video encoding, the pipeline software now only supports single jobs on the same server. We could move to container-based solutions.
* support to update an event, e.g. if there's a new version of the video file or other metadata changed
* replace [lambdacd](https://lambda.cd) with a better-maintained workflow system.
* update processing "pipeline scripts" to use newest versions of tools like FFmpeg, these are bash scripts calling FFmpeg and other tools
* find a way to update Voctoweb from official sources and keep our own design and resources, see [another idea](/#/projects?project=voctoweb:_split_contents_and_logic) for details.
* add schedule.xml support to the uploader. Schedule.xml is a file exported by talk management software like Frab or Pretalx and already contains all important information about the video of the talks.
* potential rewrite of uploader and pipeline software, if it is too complicated to add features or changes to the existing tools.

## Milestones

### Before applications

Get in touch with us to talk about potential projects we can derive from this idea. You're also invited to check out the software projects and try to get them running.

You are free to define the scope with your proposal, so it will be possible to do that project as a full-time (350 hours) or a hafl-time(175 hours) project. It is also possible to split that idea up into several projects.

### Community bonding

Use the bonding period to see the existing projects. Talk to us to learn how it works, how the workflow is, and how to make changes. During this period we will be able to identify things to work on. This can result in tasks to improve existing software or we find out that it is more effective to create something new.

### Coding period

During this period we'd like to work in an agile mode and use a Scrum or Kanban or something in between to organize the workflow. If you have questions on this, please don't hesitate to ask.

Of course, milestones will heavily depend on the idea we want to implement together. But in general, there should always be milestones like

* Build and present the first prototype for a new feature
* extend the feature to fully cover the idea
* provide tools to monitor the new feature
* create end-user documentation
* deploy the feature to production
