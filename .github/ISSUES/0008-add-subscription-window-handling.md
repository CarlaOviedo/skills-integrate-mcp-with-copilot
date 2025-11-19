**Add subscription window handling**

Description
-----------
Respect subscription windows for events using `initialSubscriptionDate` and `limitSubscriptionDate`. Prevent signups outside the open window and show clear messaging.

Acceptance criteria
-------------------
- Event model fields for `initial_subscription_date` and `limit_subscription_date`.
- Backend checks to allow signup only within the allowed window.
- UI messaging showing when signups open/close.

Labels: backend, frontend
Estimate: small
