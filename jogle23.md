# Project Proprosal
## Idea
The project being proposed is a lightweight desktop messaging app focused on providing easy access for people hosting their own messaging chats and groups. This will be done through both a server-side version and client-side version.

## Objective
The overall goal of this app is to provide an alternative to messaging apps, such as Discord and Slack, which are extremely resource heavy and privacy invasive. Discord, on average, can take up close to 1gb of ram when in use which can make it unusble on devices with 8gb of ram. Considering the cost of computers, especially RAM, presently, it is now more important than ever that apps have a focus on requiring as minimal resources as possible while providing a good user experience. Consumers shouldn't be required to upgrade their device due to not being able to run their communication app.

## Features
The main feature set will be allowing a person with an extra computer or rasberry pi lying around to setup the server which will be able to host as many chats as possible (hardware based). Friends wanting to join these chats will just need to download a client-side version of the app and setup a local account.

Core Features:
- easy to setup Self-hosting servers 
- minimal resource requirement (no more than 300mb client-side version)
- Users able to join multiple servers
- Community Chats will be able to have different group chat sections, calendar, and list of community members
- Users will be able to send images and files
- Calendar events

Privacy Features:
- no email/online account requirement

## Frameworks and Languages
The messaging app will be built using C++, Python, and SQL/SQLite. Due to one of the main goals being efficiency, C++ will handle the backend of messaging, network connections, and data encoding. Python with the framework Pyside, built off of Qt framework, will be used for the frontend GUI. This will provide both a pleasing UI and performance enchancemets compared to commonly used frameworks such as Electron. For server-side database, SQL language will be implemented due to its robustness as a framework and being industry standard.  

## Intended Users
The focus user group will consumers who want an increase in both privacy of their messages, and those with older computer hardware. We expect users who plan on hosting the servers will have some level of experience working on servers. The goal is to make the process easy as possible, but understanding some of the terminology will still be important. Our second group, people using older hardware, is a continuously growing group of people. I believe this is an extremely important group to consider more due to the cost of hardware shooting up dramatically over the past few years. Current apps tend to use frameworks such as Electron (both Discord and Slack), which is known to soak up RAM and CPU. One of the bigger complaints I read on online forums is how opening a simple messaging app can slow down workflows and feel laggy on hardware 3-5 years old (especially true for lower RAM devices). I believe this app can feel in that gap that the main messaging apps have left open.
