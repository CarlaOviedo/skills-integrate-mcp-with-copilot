**Add role-based permissions & roles**

Description
-----------
Introduce roles (admin, coordinator, teacher/docente, student) and enforce role-based access control in routes and UI.

Acceptance criteria
-------------------
- Add role field to `User` model and seeding helper to create at least one admin/coordinator.
- Middleware or dependency checks to protect endpoints based on roles.
- Show/hide UI elements based on role (basic conditional rendering is fine).

Labels: backend, security, enhancement
Estimate: small
