# TargetTrack — Recruiting & Application Dashboard

## Project Overview

TargetTrack is a web-based recruiting platform designed to help students stay organized and proactive during the internship and job search process. Users can create a list of target companies, define the types of positions they are looking for, and monitor those companies for relevant openings. When a matching opportunity is detected, the user receives a notification and can add the position to their application tracker.

## Problem

Finding and managing internship applications can be surprisingly time-consuming. Existing tools are useful for finding and organizing jobs, but they generally focus on searching broadly across many opportunities or tracking jobs after the user finds them. Our goal is to take a more focused approach: **let users identify the companies they specifically want to work for and actively monitor those companies for relevant opportunities.**

This is a problem I currently experience myself. I use a spreadsheet to manually track companies and applications, and I spend roughly 30 minutes each day checking career pages and updating my spreadsheet. Many existing tools either place useful functionality behind paid plans or do not provide the specific company-focused monitoring and notification workflow I need. TargetTrack would bring this process into one centralized application.

## Major Features

- **Company Watchlist:** Add, edit, remove, and prioritize target companies.
- **Job Preferences:** Define desired roles, keywords, locations, employment type, and recruiting period.
- **Job Monitoring:** Monitor supported career sources for new job postings.
- **Job Matching:** Filter newly discovered positions based on user preferences.
- **Smart Notifications:** Notify users about new matching positions and upcoming deadlines.
- **Application Tracker:** Track applications through statuses such as Saved, Applied, Assessment, Interview, Offer, and Rejected.
- **Dashboard:** Provide an overview of watched companies, new opportunities, applications, interviews, and upcoming deadlines.

## Technologies

### Backend
- C#
- ASP.NET Core Web API
- Entity Framework Core
- PostgreSQL

The backend will provide the REST API, manage application data, and handle scheduled background jobs for monitoring supported career sources.

### Frontend
- React
- TypeScript
- HTML/CSS

The frontend will provide the dashboard, company watchlist, job listings, application tracker, and notification interface.

### Development & Infrastructure
- Docker
- Git/GitHub
- Swagger/OpenAPI

### Job Monitoring & Notifications
- Career-site/ATS APIs where available
- HTML parsing where appropriate
- In-app notifications
- Potentially an email service such as Resend

## Intended Users

The primary users are college students searching for internships or entry-level positions, particularly students targeting many specific companies. These users would benefit from having one place to manage their search and receiving timely notifications when companies they care about post relevant opportunities. The platform is intended to reduce the need to repeatedly check dozens of career pages, replace manual spreadsheets, and make the recruiting process more organized and proactive.