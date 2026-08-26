

## Proposal: Leftover Link

The project I'm proposing is called Leftover Link. It is a system that helps campus organizations and local businesses notify students when usable food is left over after events. It aims to both reduce food waste and prevent students from going hungry.

After campus events, meetings, or business functions, extra food may still be completely usable but get thrown away because there is no quick way to connect it with people who want it. Leftover Link would create that connection by giving organizations and businesses one central place to share what is available. Students could then find nearby food while there is still time to pick it up.

Features include the following:

- Organizations can post available food, quantity, deadline, and location.
- Students can set up notifications and view the offers on a feed-like page.
- Offers automatically expire at their deadline.
- Users can filter offers for allergens or dietary needs.
- A dashboard can track the estimated amount of food diverted from waste.

The posting process should be fast and simple so that an organization can create an offer immediately after an event. Including the quantity would help students understand how much food is left, while the location and pickup deadline would tell them where to go and how quickly they need to respond. Automatic expiration would keep the feed current instead of showing food that is no longer available. Dietary filters would also make the system more useful to students who need to avoid certain ingredients.

I would plan to use React, Python/FastAPI, SQLite, a mapping API, and optional email or text notifications.

React would provide the user-facing feed and posting forms, while Python and FastAPI would handle the application's main logic. SQLite would store offers and user information, and the mapping API would help students identify nearby pickup locations. Email or text notifications could alert students when a relevant new offer is posted.

The intended users would be students and those with extra food. This is something useful for both parties. There's nothing students love more than free food, and it's always wonderful to avoid wasting food and to help others.
