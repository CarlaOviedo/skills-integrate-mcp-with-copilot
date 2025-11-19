**Add persistent database and ORM models**

Description
-----------
Replace the current in-memory `activities` storage with a persistent database and ORM models. Introduce models and migrations for core entities: `Event`, `User`, `Student` (if separate), `Category`, `Campus`, and `Status`.

Acceptance criteria
-------------------
- Add a database dependency and configuration (SQLite for local development; Postgres optional).
- Create ORM models and migrations for `Event`, `User`, `Category`, `Campus`, and `Status`.
- Update code to read/write activities from the DB instead of the in-memory `activities` dict.
- Provide a short developer README section describing how to run migrations and configure the DB.

Labels: backend, database, enhancement
Estimate: medium
