# Smart Scheduling/Meet Organizer Proposal

## Brief summary  
My proposal for the cs340 group project is a scheduling app that allows groups to coordinate their events. The app would allow users to show their availability to other people in their group, their preferred times, deadlines, and upcoming events in an easy to understand format.

##Problem it solves  
This app solves the problem of convoluted schedules due to miscommunication between group members. It also makes the process easier so you don’t have to learn how to use something like excel or so you are not constantly changing event times because it doesn’t work for someone.

## Features

- Create an event (title, description, duration, date range, timezone)  
- Generate shareable invite link (join as participant)  
- Participant availability input on a weekly grid (drag/click to mark times)  
- Optional availability levels: Available vs Preferred  
- Participant list with completion status (who has submitted availability)  
- Compute and rank best meeting times (top N suggestions)  
- Results view with scores (e.g., attendance count / preference score)  
- Finalize a time and lock the event  
- Export finalized meeting as preferred file type

## Target Audience  
This app is mainly for mid to large size groups that are looking to make scheduling easier and efficient. Could also be for people that are looking for a new calendar app to keep track of their upcoming events.

## Project Reqs.

- Frontend software (e.g. React, Vite, tailwind css)  
- Backend software (e.g. Python FastAPI, JWT)  
- Optimization/Scheduling engine (Google OR-Tools)  
- Database & Storage (PostgreSQL)  
- Integration and File Formats (ICS, google calendar)  
- Deployment (docker)  
-Testing
