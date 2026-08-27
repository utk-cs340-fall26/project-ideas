# Smart Study Planner — Project Proposal

## Brief Summary
The Smart Study Planner is a web-based application designed to help college students manage their academic workload. Users can enter their courses, assignments, exams, deadlines, estimated workloads, and available study times. The application will then generate a personalized study schedule that prioritizes tasks based on urgency, workload, and importance. Unlike a traditional calendar, the planner can adjust the schedule when tasks are completed late or new assignments are added.

## 1. What Problem It Solves

College students often have multiple assignments, exams, and projects competing for their limited time. Traditional calendars can show students what is due but do not necessarily help them determine when they should work on it. The Smart Study Planner addresses this problem by organizing academic responsibilities in one location and automatically creating manageable study sessions. It will help students prioritize deadlines, balance workloads between courses, and adapt their schedules when plans change.

## 2. Major Features
* Course and assignment management
* Assignment and exam deadline tracking
* Estimated workload and priority settings
* User-defined study availability
* Automatic study schedule generation
* Daily and weekly calendar views
* Task completion tracking
* Automatic rescheduling when time permits
* Optional workload and progress visualization

The core scheduling system will be completed before advanced features are added.

## 3. Technologies

The project will use Python with Flask for the backend and JavaScript, HTML, and CSS for the frontend. SQLite and SQLAlchemy will be used to store and manage user, course, assignment, and schedule data. FullCalendar will provide the calendar interface, while pytest will be used for automated testing. Git and GitHub will support version control and collaboration.

The scheduling algorithm will be developed by the team rather than relying on an external scheduling service. This will allow the project to demonstrate concepts such as prioritization, constraint handling, and optimization.

## 4. Intended Users

The primary users are college and university students, particularly those managing multiple demanding courses. Students would benefit from having one application that not only tracks their deadlines but also determines how to use their available study time effectively. By automatically creating and adjusting study sessions, the Smart Study Planner can reduce the effort required to organize academic work and help students stay on track throughout the semester.
