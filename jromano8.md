# Project Proposal: Network Security Assistant

## Project Summary

This project is a user-friendly network security assistant designed to help home users and small businesses understand and improve the security of their local networks. The application will scan an authorized local network, identify connected devices, analyze network structure, and highlight potential security and segmentation issues. Rather than presenting users with complex networking terminology, the application will translate technical findings into clear explanations and actionable recommendations.

## Problem

Many home networks and small businesses have limited cybersecurity knowledge and resources. Users may not know which devices are connected to their network, whether unknown devices are present, or whether computers, IoT devices, guests, and other systems are properly separated. Existing network-scanning and management tools can also be intimidating for nontechnical users. This application aims to provide an accessible way to gain network visibility and identify common security weaknesses without requiring a dedicated network or cybersecurity professional.

## Major Features

- Automated discovery and inventory of devices on an authorized local network
- Detection of IP addresses, MAC addresses, hostnames, and device manufacturers when available
- Identification and analysis of local subnets and network interfaces
- Visualization of discovered devices and network topology
- Identification of potential network segmentation issues
- Authorized connectivity/reachability testing between network segments where technically possible
- User-friendly security health score and prioritized recommendations
- Plain-language explanations of security findings
- Detailed views for technically knowledgeable users
- Exportable network and security reports

## Technologies

The frontend will use **React and TypeScript**, along with HTML and CSS, to provide an interactive dashboard and network visualization. The backend will be developed with **C# and ASP.NET Core Web API**, providing REST endpoints, authentication, scan management, security analysis, and application logic. **Entity Framework Core (EF Core)** will serve as the application's object-relational mapper, while **Microsoft SQL Server** will store users, networks, devices, scan results, VLAN information, and security findings. A lightweight **network scanning agent** will run on an authorized computer within the network and communicate scan results to the ASP.NET Core API. Networking functionality will use appropriate C# networking libraries and operating-system networking utilities. **Docker**, **Git/GitHub**, **Swagger/OpenAPI**, and **xUnit** will support deployment, collaboration, API documentation, and automated testing.

## Intended Users

The primary users are **home network owners and small-business owners or IT personnel** who lack dedicated cybersecurity staff. These users want an inexpensive and understandable way to see what is connected to their network and identify potential security problems. By combining automated technical analysis with simple explanations and recommended actions, the application will help users make better-informed security decisions without requiring advanced networking knowledge.
