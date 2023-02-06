---
name: "El Repo.io desktop client"
desc: "Compile the actual flutter app into a desktop client using electron or native app"
requirements:
 - "Flutter knowledge"
difficulty: "medium"
size: "175 hours"
mentors:
 - nicoechaniz
 - G10h4ck
initiatives:
 - GSoC
 - GSoC2023
tags:
 - GSoC
 - RetroShare
 - Decentralized
 - Culture sharing
collaborating_projects:
 - Altermundi
---

[ElRepo.io](https://elrepo.io) is a decentralized repository of culture built on RetroShare API client. 
The actual app is developed with Flutter and supports Android systems. However, Flutter framework gives
the possibility to build apps to different platforms from a single codebase.

- One possibility is to experiment how to pack a flutter web app into an Electron app to distribute it 
as desktop app.

- Other one is experiment with Flutter native desktop framework to distribute a binary for each platform.

#### Milestones

- Knowing basic of how Flutter and Dart work is needed. 
- Create a plugin capable to interact with RetroShare for each platform (start, stop it, bundle it)
- Create different versions of the app and check what is the fastest way to distribute a multiplatform package.
