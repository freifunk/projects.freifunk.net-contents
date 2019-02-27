---
collaborating_projects:
  - freifunk
desc: ""
developers_involved:
  - andibraeu
  - christian-draeger
difficulty: medium
status: open
email: ab+gsoc2018@andi95.de
initiatives:
  - GSoC
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
  - GSoC2019
  - json
  - web
  - voctoweb
  - video
---

## About our videoodyssee

In 2017 we started our own video portal for freifunk at [media.freifunk.net](https://media.freifunk.net). To get videos online we have a more or less complicated upload workflow:

1. upload video file to a processing server
2. correct video file settings
3. convert video to target formats
4. upload to CDN and Youtube
5. publish at the media portal

## Provided services

The following systems are involved:

1. [Videoodyssee Uploader](https://github.com/christian-draeger/videoodyssee-uploader) - a web portal to upload video files built with Spring Boot, Thymeleaf, CSS, JS, Ansible and Maven
2. Videoodyssee - the processing server, built with bash scripts and python
3. [lambdacd pipeline](https://github.com/freifunk/videoodyssee.freifunk.net-ci/) - controls the workflow, built with clojure, leiningen and LambdaCD
4. [mirrorbits](https://github.com/etix/mirrorbits) - the CDN, built with Go
5. [voctoweb](https://github.com/freifunk/voctoweb) - the media portal, built with Ruby, HTML, CSS, JS and puma

As of now it is possible to upload new videos, but the process is not comfortable. So we need to improve the software.

## Ideas for changes

There are already some ideas for improvements:

* add publishing workflow to prevent publishing of unwanted videos (e.g. send an email to a group of people to unlock the video)
* refactoring the uploader project to use a message based frontend to backend system, e.g. by using Spring Webflux, React or Websockets
* support multiple workers for video encoding, the pipeline software now only supports single jobs on the same server.
* support to update an event, e.g. if there's a new version of the video file or other meta data changed
* elaborate lambdacd api to get feedback in uploader, so you can see progress in the workflow on the web portal.
* update processing "pipeline scripts" to use newest versions of tools like ffmpeg, these are bash scripts calling ffmpeg and other tools
* find a way to update voctoweb from official sources and keep our own design and resources
* add schedule.xml support to uploader. Schedule.xml is a file exported by talk management software like frab or pretalx and already contains all important information about the video of the talks.
* potential rerwite of uploader and pipeline software, if it is too complicated to add features or changes on the existing tools.
