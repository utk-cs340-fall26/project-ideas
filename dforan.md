# Project Idea - Lost and Found Messaging Board

## Project Summary
The Lost & Found Board is a web application that allows members of a campus community to post about items they have lost or found and to search through existing posts to find matches. Users can create an account, submit a post with a photo and description, and browse or filter through all active posts to locate their belongings or return items to their rightful owners. The application focuses on being simple, fast to use, and reliable.


## Problem It Solves
Every semester, students and staff misplace personal items such as water bottles, backpacks, ID cards, chargers, and textbooks, and there is currently no centralized, easy-to-search system for reporting or locating them on campus. Physical lost-and-found offices are often inconvenient to check, have limited hours, and require users to travel across campus just to see if their item has been turned in. This project solves that problem by creating a digital, always-accessible board where lost and found items can be posted, searched, and claimed from any device, reducing the time and effort required to reunite people with their belongings.

## Major Features
- User registration and login so posts are tied to specific accounts, allowing the poster to mark missing items as resolved.
- Ability to create posts for either a lost item or a found item, including information such as location (building, room # etc...), a photo upload, a written description, and the date the item was lost or found.
- Searchable and filterable board that allows users to browse posts, and narrow results based on category, date range, location, and whether the item was lost or found.
- View for individual posts with more information, and allows users to view contact information for the poster.
- Ability for a poster to mark their post as resolved, removing the post from searchable or filterable results.

## Technologies
- Frontend: React with a CSS framework to build the browsing, serach, and posting interface.
- Backend: Python with Flask to handle application API, authentication, and logic.
- Database: PostgreSQL.
- Image Storage: Cloud storage service such as Amazon S3.
- Authentication: Library such as Passport.js

## Intended Users
The intended users are college students, faculty, and staff who regularly move through a shared campus environment and are at risk of losing or finding personal items throughout the day. Students in particular would want to use this application because it gives them a fast, self-service way to check for their lost belongings without needing to physically visit a lost-and-found office during specific hours. Faculty and staff would benefit as well, since they could use the platform to quickly report items found in classrooms, offices, or common areas, helping return them to their owners with minimal effort. Overall, the application appeals to anyone who wants a more convenient, transparent, and immediate alternative to traditional lost-and-found systems.