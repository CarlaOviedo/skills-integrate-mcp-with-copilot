---
name: "Review REMS (bearlike/REMS-For-Organisations) — features audit"
about: "Audit the REMS repo for features we might adopt or adapt"
title: "Review REMS (bearlike/REMS-For-Organisations) — features audit"
labels: ["audit", "research"]
assignees: []
---

## Summary

We previously inspected `bearlike/REMS-For-Organisations` and identified features relevant to our project: bulk mailer, certificate generator, registration workflow, admin dashboard, templates, and Docker packaging. This issue tracks a focused audit of those areas so we can decide which to adopt or adapt into `CarlaOviedo/skills-integrate-mcp-with-copilot`.

## Acceptance criteria

- [ ] Read `src/app/routes/certificates.py` and document how certificates are generated (templating + PDF generation tool).
- [ ] Read `src/app/utils/email.py` and confirm which mail provider / SMTP method is used and whether templated bulk sends are supported.
- [ ] Enumerate DB models in `src/app/models.py` that are relevant (members, events, registrations, certificates, mails) and map them to our data model.
- [ ] Verify public registration flow by inspecting `src/app/routes/public.py` and the registration template `src/app/templates/forms/registrations.html`.
- [ ] List any external dependencies required (from `requirements.txt` or `pyproject.toml`) needed to run certificate generation or mailing features.
- [ ] Produce a short recommendation (keep/adapt/reimplement) for each feature with an estimated level-of-effort.

## Notes

- Repo inspected: `bearlike/REMS-For-Organisations` (https://github.com/bearlike/REMS-For-Organisations)
- Suggested next steps after this audit: implement mailer prototype, integrate certificate generation pipeline, and add sample deployment (Docker Compose).

## Checklist (implementation tasks)

- [ ] Create a branch `feature/rems-audit` and add documentation of findings to `/docs/rems-audit.md`.
- [ ] If we choose to adopt, open separate implementation issues for `bulk-mailer`, `certificates`, and `registration-workflow`.

<!-- Draft issue file created by assistant. -->
