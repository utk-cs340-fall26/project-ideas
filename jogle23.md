# Project Proprosal
## Idea
The project being proposed is a lightweight desktop messaging app focused on providing easy access for people hosting their own messaging chats and groups. 

## Objective
The overall goal of this app is to provide an alternative to messaging apps, such as Discord and Slack, which are extremely resource heavy and privacy invasive. Discord, on average, can take up close to 1gb of ram when in use which can make it unusble on devices with 8gb of ram. Considering the cost of computers, especially RAM, presently, it is now more important than ever that apps have a focus on requiring as minimal resources as possible while providing a good user experience. Consumers shouldn't be required to upgrade their device due to not being able to run their communication app.

## Features
Chat Features:
- easy to setup Self-hosting servers 
- minimal resource requirement (no more than 300mb)
- Users able to join multiple servers
- Servers will be able to have groupchats, calendar, and list of community members
- Users will be able to send images and files
- Calendar events

Privacy Features:
- easy setup process for hosting personal servers
- no email/online account requirement

## Frameworks and Languages
The messaging app will be built using C++, Python, and SQL/SQLite. Due to one of the main goals being efficiency, C++ will handle the backend of messaging, network connections, and data encoding. Python with the framework Pyside, built off of Qt framework, will be used for the frontend GUI. This will provide both a pleasing UI and performance enchancemets compared to commonly used frameworks such as Electron. For server-side database, SQL language will be implemented due to its robustness as a framework and being industry standard.  

