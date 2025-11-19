**Add event moderation / approval workflow**

Description
-----------
Implement a moderation workflow where events submitted by users are set to `Pending` and must be approved or rejected by course coordinators or admins before appearing on the main mural.

Acceptance criteria
-------------------
- Add `status`/`statusId` field to Event model with at least `Pending`, `Approved`, `Rejected` statuses.
- Coordinator/admin endpoints/UI to approve/reject events with comments.
- Pending events are not visible in the public event list until approved.

Labels: backend, feature, workflow
Estimate: small
