# The Idea

An app that connects to your email and automatically tracks the status of your job applications. Instead of manually updating a spreadsheet every time you hear back from a company, the app scans your inbox, matches replies to the applications you've logged, and figures out whether you've been rejected, ghosted, invited to interview, or offered the job.

# The Problem It Solves

Anyone applying to a lot of jobs ends up losing track of where things stand. Some companies reply fast, some take months, and a lot never reply at all. Manually checking dozens of email threads and updating a tracker by hand is tedious, and it's easy to lose track of which applications are still live versus quietly dead. This app removes that manual work by watching for replies and updating status automatically, including catching a late rejection or interview invite for an application that had already been marked as ghosted.

# Major Features

- A simple form to log each application: company, role, and date applied
- Read-only inbox scanning that matches incoming emails to logged applications by sender domain, company name, or subject line
- Automatic status detection: Pending, Ghosted, Rejected, Interview, or Accepted
- A configurable ghosting window (default 30 days with no reply) that updates automatically if a late response comes in
- Hybrid email classification: fast keyword rules catch common rejection phrasing, with a fallback for anything ambiguous
- A dashboard showing response rate, average time-to-response, ghosting rate by company, and an application funnel from applied to interview to offer or reject

# Technologies

- Backend: Python or Node.js
- Email access: Gmail API with read-only OAuth scope
- Classification: keyword/regex rules for clear cases, LLM API call for ambiguous emails
- Database: PostgreSQL or Supabase
- Frontend: React or React Native, depending on whether this ships as a web app or mobile app

# Who the Intended Users Are

The core audience is job seekers who are applying broadly, especially students and new grads sending out large volumes of applications during a hiring season. That volume is exactly what makes manual tracking break down. These users want to know where they actually stand without digging back through their inbox, and they want a system that keeps working even after they've written an application off as ghosted. A secondary use case is anyone who wants better visibility into their job search overall, since the dashboard surfaces patterns, like which types of companies tend to ghost, that are useful for deciding where to focus future applications.