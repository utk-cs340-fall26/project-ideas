# Project Proposal: Ember — A Shared Habit & Task Tracker (Mobile-First Web App)

## A Brief Summary

#### Ember is a mobile-first app that helps people build and stick to habits by making progress visible and, critically, shared. Instead of another solo checkbox app, Ember lets users track personal habits and tasks while optionally forming small accountability groups — roommates, study partners, teammates — who can see each other's progress and cheer each other on. Users get adaptive streaks (a streak that smolders and can be reignited instead of being wiped out by one bad day), calendar-style progress views, and a weekly summary that highlights patterns in their behavior, not just raw completion counts. Ember is built as an installable Progressive Web App (PWA), which lets us deliver a genuine mobile experience — home screen install, offline check-ins, push notifications — using web technology.
---
## What problem it solves

#### Most habit trackers fail for the same reason diets fail: motivation drops off after a week or two once the novelty wears off. Existing apps are largely solo experiences — you check a box, you see a number go up, and that's it. There's no social pressure, no context for why you're slipping, and no forgiveness when life happens and you miss a day. People don't need another glorified to-do list; they need something that keeps them accountable, fits naturally into their day, and actually helps them understand their own patterns.
---
## A list of major features

 - Habit & task creation — recurring habits (daily/weekly) and one-off tasks, with categories and custom targets
 - Daily check-ins — fast, low-friction logging with streak tracking
 - Adaptive streaks — instead of a hard reset on one missed day, streak "health" decays gradually and recovers with consistency, so one bad day doesn't erase weeks of progress
 - Group accountability — users can form small groups and share specific habits, seeing teammates' check-ins on a shared view
 - Progress dashboard — calendar heatmap, completion percentages, and trend charts
 - Weekly insight summary — an auto-generated recap identifying which habits are strongest, which are slipping, and simple correlations (e.g., workout completion is higher on days sleep goals are also met)
 - Push notifications — habit reminders delivered at the right time of day to reduce missed check-ins
 - Installable home screen app — added to the home screen like a native app, launches full-screen, no app store required
 - Email and Password Login — traditional login method, have the device
 - Persistent login — sign in once and stay logged in on your device via secure refresh tokens, no biometric hardware required and no need to re-enter credentials each session (with the ability to log out remotely if a device is lost)

---
## Technologies you plan to use (languages, tools, third-partyAPIs/libraries)

 - Frontend: React with Vite, built as a PWA (service worker + web app manifest) for installability and offline support
 - Local storage / offline support: IndexedDB (via a lightweight wrapper like Dexie.js) to queue check-ins offline and sync automatically when connectivity returns
 - Backend: Node.js with Express, REST API architecture
 - Database: PostgreSQL for structured relational data (users, habits, check-ins, groups)
 - Auth: JWT-based authentication, with optional WebAuthn biometric login layered on top for supported devices
 - Notifications: Web Push API (via a service like OneSignal, or the native Push API + service worker) for habit reminders
 - Insights: lightweight use of an LLM API (e.g., OpenAI) for generating weekly natural-language summaries, called on a scheduled batch job rather than in real time to keep costs predictable
 - Deployment: Frontend on Vercel or Netlify, backend + database on Render or Railway — all reachable instantly via a URL, with no app store review process to slow down our timeline
---
## Who the intended users are and why they would want this

#### Our primary users are students and young professionals trying to build consistency in busy, unpredictable schedules — people who've tried habit apps before and abandoned them. Ember meets them where habit-building actually happens: on the go, between classes, at the gym, without needing to open a laptop. Roommates and study groups are a natural early user base since the group-accountability feature solves a real gap: most trackers assume you're doing this alone, when in practice, shared goals (working out together, studying together) are often easier to stick to than solo ones. The forgiving streak system, push reminders, and weekly insights also target users who've felt punished or discouraged by rigid all-or-nothing tracking in existing apps.
---