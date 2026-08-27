# StudySpot — Project Proposal

## The idea

StudySpot is a live seat map for campus study spaces. Every table gets a printed QR code taped to it. You sit down, scan, say how long you're staying, and if you're alone at a multi-seat table you say whether you're open to someone joining you. That feeds a real-time map of what's actually open right now.

## The problem

During midterms and finals, finding a seat in Hodges is a scavenger hunt. You walk four floors, and the seats that are technically free are the ones nobody can use — a single person spread across a six-top, a study room with one occupant. The space exists, the information about it doesn't. Everyone loses ten to twenty minutes to guesswork, and the students who lose are usually the ones who showed up between classes with the least time to spare.

## Major features

- **QR check-in.** One code per table, generated and printed by us. Scan, set an estimated stay, done. No account setup blocking the first scan.
- **Auto-expiring sessions.** The time estimate is the checkout. Sessions clear themselves when they lapse, with a push to extend, so we never depend on people remembering to scan out.
- **Open-to-share toggle.** Sitting solo at a four-top? Mark yourself open. Now that table shows as three seats available instead of zero.
- **Live floor map** with color-coded availability per table, per floor.
- **Filters** for table size, outlets, quiet vs. collaborative zone, and open-to-share seats.
- **Report button** for wrong status, so bad data self-corrects.
- **Admin view** for printing and reassigning table codes.

## Technologies

React with TypeScript on the frontend. Floor maps are hand-built SVGs with each table as a clickable element keyed to a table ID — simpler and more reliable than trying to source real blueprints. Node/Express backend, PostgreSQL for tables and sessions, with expiration handled by a timestamp column and a cleanup job. QR codes generated with the `qrcode` npm library, encoding a table ID that deep-links into the web app. UT email auth via SendGrid. Hosted on Render and Vercel.

## Who it's for

UTK students during high-demand hours, and secondarily the library staff, who currently have no occupancy data at all. Students use it because the payoff is immediate and selfish: scan once, and the map you just helped build is the one that finds you a seat next Tuesday.

Pilot one floor of Hodges, prove the data holds, then expand.
