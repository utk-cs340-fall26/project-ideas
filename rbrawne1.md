# Project Proposal

## Project Summary

My project proposal is for a lost and found application that any community can use to help people who have lost items easily locate their items that they lost in the area. On the user end, they would have an account linked to separate communities they're in where they can submit a request for a lost item that has been turned in by giving details on the item. On an admin's end, they would have a list of pictures of each item that's been turned in that they can cross reference with the details the user gave, and be able to send a picture back to the user to verify if an item that matches the description is the item the user was looking for. The admin can then respond with where the user can pick up the item.

## Problem it solves

It streamlines the process of retrieving a lost item on both the user and admin's end. Instead of having to look through items physically where they may be hard to spot if they're smaller items like keychains or pens, the admin only has to scroll through photos until they can find something that matches. The user, if they're already a part of the community, just has to submit a request to pick up the item with the necessary details so the admin can verify.

## Major features

- User accounts and login system
- User roles (community member and community admin)
- Grouping various accounts and ability to join multiple groups
- Item storage and statuses
- Some basic communication implementation
- Small security checks (such as checking in when arriving to pickup an item)

## Potential technology needed

- React for frontend
- Python FastAPI for backend
- Supabase Postgres for database
- Supabase Auth for authentication
- Supabase Storage for storage

## Who the intended users would be

THe intended user for this would be someone who lives in a community that is large enough to be impersonal such as UT's campus or a larger neighborhood where everyone may not know everyone else in the community. 