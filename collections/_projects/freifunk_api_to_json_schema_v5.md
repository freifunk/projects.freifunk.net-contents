---
collaborating_projects:
  - freifunk
desc: "Update the API Schema and our tools to json draft v5"
developers_involved: []
difficulty: medium
status: open
initiatives:
  - GSoC
issues:
  - "https://github.com/freifunk/api.freifunk.net/issues/145"
markdown: freifunk_api_to_json_schema_v5.md
mentors:
  - andibraeu
name: "Update Freifunk API JSON schema"
requirements:
  - "Analyzing and coding"
  - "identify components that must be changed"
  - "refactoring, migrations"
  - "javascript, python, php, wordpress plugins"
tags:
  - json
  - web
  - map
  - collectors
  - communities
---

When we created the freifunk API some years ago, json schema v3 draft was en vogue. If you want to know more about the freifunk API, see https://api.freifunk.net

Goal is to update our schema and the depending tools to the newer v5 draft. The schema version is already contained in our schema files. So tools that use these schema files can be backwards compatible until every community updated their api files. The api viewer contains a validation of api files: https://github.com/freifunk/viewer.api.freifunk.net/blob/master/render.py#L76 This should be used in the community collector, too.

Tools we created are:

* API generator to generate a new API file: https://freifunk.net/generator
* the community map: http://community.freifunk.net
* RSS feed aggregator
* community collector (to collect all api files and summarize it)
* the api viewer
* betterplace donations table
* freifunk-karte.de
* more to find.

a lot of these tools use the summarized file produced by the community collector.

#### Milestones

##### PREPARATION/BONDING

- A clear understanding of JSON Schema
- found the components that need to migrated or refactored
