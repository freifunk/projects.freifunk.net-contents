# projects.freifunk.net-contents
contents to be displayed at our projects-page

preparations:

* install ansible
* run ```ansible-playbook deploy_coala-projects.yml -i path-to-your-inventory --limit "the server to deploy to" --extra-vars "install_user=your-install-user install_path=/path/to/install"```


## Defining Projects

Mentors and admins can define projects in markdown using the following structure and save it in the collections/_projects folder with a relevant filename:

```
---
name: "Write Project Name Here"
desc: "Write a one line Description of Project here."
requirements:
 - "The applicant has to fulfill this to get started."
difficulty: "low|medium|high"
issues:
 - "https://github.com/coala/coala/issues/####"
mentors:
 - sils
 - sims1253
initiatives:
 - GSoC
tags:
 - Plugins
 - CI
collaborating_projects:
 - "Add umbrella and sub-orgs here"
---

This space is for the main description. Use it wisely.

#### Milestones

##### GSOC 2017 COMMUNITY BONDING

* Conceptual work should be finished.
* The student have a repository, know how to work with the community.
* The applicant should know the community.

##### GSOC 2017 MIDTERM

* Everything listed here has to be reviewed and merged by midterm.
* No exceptions to that. Changing the goals is possible together with mentors.
* Yes, that includes tests and documentation.

##### GSOC 2017 FINAL

* Everything has to be reviewed and merged.
* Including tests and docs, again.

```

## Defining FAQs

Users can also add FAQs by simply creating a markdown file in collections/_faq folder.

Format for faq markdown file is as follows:
```
---
Question: <Write the question here>
---

Answer
```
