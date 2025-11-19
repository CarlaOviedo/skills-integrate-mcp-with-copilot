**Add file uploads for event photos & official documents**

Description
-----------
Support uploading event photos and official authorization documents. Provide local disk storage by default and document how to switch to S3 (optional).

Acceptance criteria
-------------------
- Backend endpoints to accept file uploads and associate them with the `Event` record.
- Store files on local disk under a configured directory and serve them safely.
- Frontend support for uploading files when creating/editing events.

Labels: backend, storage, enhancement
Estimate: small
